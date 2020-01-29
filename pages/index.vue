<template>
  <sectionList :sections="sections"/>
</template>

<script>
import sectionList from '~/components/sectionList'

export default {
  components: {
    sectionList,
  },
  
  data: () => ({
    sections: [
      {type: 'pageHeading'},
      {type: 'imageLinks'},
      {type: 'imgArticle'},
      {type: 'products'},
      {type: 'advantages'},
      {type: 'gallery'},
      {type: 'faq'},
      {type: 'news'},
    ],
  }),

  computed: {
    path() {
      return ''
    }
  },
}
</script>
