<script setup>
import {siteConfig as c} from '../config/siteConfig';
import Icon from './Icon.vue';
</script>
<template>
  <div class="google-reviews-card">
    <p class="eyebrow">AVALIAÇÕES NO GOOGLE</p>
    <h3>{{ c.googleReviews.businessName }}</h3>
    <p>{{ c.googleReviews.location }}</p>
    <p class="google-review-count"><strong>{{ c.googleReviews.count }}</strong> avaliações no Google</p>
    <p>Conheça as experiências compartilhadas pelas clientes diretamente no Google.</p>
    <a :href="c.contact.reviewsUrl" target="_blank" rel="noopener noreferrer" class="button">Ler avaliações no Google <Icon name="arrow" /></a>
    <small>{{ c.googleReviews.countSource }} em {{ c.googleReviews.countDate }}. Consulte a contagem atual no Google.</small>
  </div>
</template>
