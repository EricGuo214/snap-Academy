<script setup>
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import SupportIcon from './icons/IconSupport.vue'
</script>

<template>
  <WelcomeItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>Spring rolls $15.99</template>

    <img alt="Food" class="logo" src="https://newmandarinca.com/images/1.jpg" width="300" height="300" />
  </WelcomeItem>

<WelcomeItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>Fish cake $14.50</template>

    <img alt="Food" class="logo" src="https://newmandarinca.com/images/2.jpg" width="300" height="300" />
  </WelcomeItem>

<WelcomeItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>Shrimp $13.50</template>

    <img alt="Food" class="logo" src="https://newmandarinca.com/images/3.jpg" width="300" height="300" />
  </WelcomeItem>


</template>
