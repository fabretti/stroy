<template>
  <main>
    <template v-for="(section, index) in sections">
      <pageHeading
        v-if="section.type == 'pageHeading'"
        :key="index"
      />
      <imageLinks
        v-else-if="section.type == 'imageLinks'"
        :key="index"
      />
      <imgArticle
        v-else-if="section.type == 'imgArticle'"
        :key="index"
      />
      <products
        v-else-if="section.type == 'products'"
        :key="index"
      />
      <advantages
        v-else-if="section.type == 'advantages'"
        :key="index"
      />
      <gallery
        v-else-if="section.type == 'gallery'"
        :key="index"
      />
      <faq
        v-else-if="section.type == 'faq'"
        :key="index"
      />
      <news
        v-else-if="section.type == 'news'"
        :key="index"
      />
    </template>
  </main>
</template>

<script>
import pageHeading from '~/components/pageHeading'
import imageLinks from '~/components/imageLinks'
import imgArticle from '~/components/imgArticle'
import products from '~/components/products'
import advantages from '~/components/advantages'
import gallery from '~/components/gallery'
import faq from '~/components/faq'
import news from '~/components/news'

export default {
  components: {
    pageHeading,
    imageLinks,
    imgArticle,
    products,
    advantages,
    gallery,
    faq,
    news,
  },
  props: {
    sections: {type: Array},
  },
}
</script>