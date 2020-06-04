<template>
  <b-container>
    <main>
      <h1>Hyperverse</h1>
      <h3>A MINECRAFT WORLD MANAGEMENT PLUGIN</h3>
    </main>
    <section>
      <b-row>
        <b-col>
          <a href="https://github.com/Sauilitired/Hyperverse" target="_blank">
            <fa :icon="github" />
          </a>
        </b-col>
        <b-col>
          <a href="https://discord.gg/KxkjDVg" target="_blank">
            <fa :icon="discord" />
          </a>
        </b-col>
        <b-col>
          <a
            href="https://www.spigotmc.org/resources/hyperverse-w-i-p.77550"
            target="_blank"
          >
            <fa :icon="download" />
          </a>
        </b-col>
      </b-row>
    </section>
  </b-container>
</template>

<script>
import { faGithub, faDiscord } from '@fortawesome/free-brands-svg-icons'
import { faDownload } from '@fortawesome/free-solid-svg-icons'

export default {
  computed: {
    github() {
      return faGithub
    },
    discord() {
      return faDiscord
    },
    download() {
      return faDownload
    }
  }
}
</script>

<style lang="scss" scoped>
main,
section {
  text-align: center;
}

main {
  color: #b0a7c7;

  h1,
  h3 {
    opacity: 0.85;
    text-shadow: 1px 3px #524c63;
  }

  h1 {
    font-family: 'Londrina Solid';
  }

  h3 {
    font-family: 'Big Shoulders Text';
  }

  @media (min-width: 320px) {
    padding-top: 64px;

    h1 {
      font-size: 64px;
    }

    h3 {
      font-size: 36px;
    }
  }

  @media (min-width: 321px) {
    padding-top: 16px;

    h1 {
      font-size: 72px;
    }

    h3 {
      font-size: 42px;
    }
  }

  @media (min-width: 576px) {
    padding-top: 46px;
  }

  @media (min-width: 768px) {
    padding-top: 46px;

    @media (min-height: 376px) {
      padding-top: 196px;
    }
  }

  @media (min-width: 1200px) {
    padding-top: 84px;

    h1 {
      font-size: 128px;
    }

    h3 {
      font-size: 64px;
    }
  }
}

section {
  a {
    color: #9284b3;

    &:hover,
    &:active,
    &:focus {
      color: #62577d;
      text-decoration: none;
    }
  }

  padding-top: 16px;
  font-size: 48px;

  @media (min-width: 576px) {
    padding-top: 24px;
  }

  @media (min-width: 768px) {
    padding-top: 32px;
  }

  @media (min-width: 1200px) {
    font-size: 84px;
  }
}
</style>
