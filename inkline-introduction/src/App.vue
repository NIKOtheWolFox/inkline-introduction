<script setup lang="ts">
import { ref } from "vue"

const inputValue = ref("")
</script>

<template>
  <i-layout>
    <i-layout-header>
      <i-navbar>
        <i-navbar-brand>Inkline Introduction</i-navbar-brand>
      </i-navbar>
    </i-layout-header>
    <i-layout vertical class="_padding-top:1/2">
      <i-layout-aside>
        <i-sidebar>
          <i-nav vertical>
            <i-nav-item>item1</i-nav-item>
            <i-nav-item>item2</i-nav-item>
            <i-nav-item>item3</i-nav-item>
          </i-nav>
        </i-sidebar>
      </i-layout-aside>
      <i-layout-content>
        <i-container fluid>
          <i-row>
            <i-column>
              <h1>Some of Inkline Controls</h1>
            </i-column>
          </i-row>
          <i-row>
            <i-column>
              <h2>Button</h2>
              <i-button>Button</i-button>
              <i-button color="primary">Primary</i-button>
              <i-button color="secondary">Secondary</i-button>
              <i-button color="success">Success</i-button>
              <i-button color="danger">Danger</i-button>
              <i-button color="warning">Warning</i-button>
              <i-button color="info">Info</i-button>
              <i-button color="light">Light</i-button>
              <i-button color="dark">Dark</i-button>
            </i-column>
          </i-row>
          <i-row>
            <i-column>
              <h2>Input</h2>
              <i-input v-model="inputValue" placeholder="Type something.." />
            </i-column>
          </i-row>
          <i-row>
            <i-column>
              <h2>Text</h2>
              <p class="_text-align:left">This is a left aligned text.</p>
              <p class="_text-align:center">This is a center aligned text.</p>
              <p class="_text-align:right">This is a right aligned text.</p>
            </i-column>
          </i-row>
        </i-container>
      </i-layout-content>
    </i-layout>
    <i-layout-footer>
      <div class="_border">(c) 2022 NIKO</div>
    </i-layout-footer>
  </i-layout>
</template>

<style>
._border {
  padding: 6px;
}
</style>
