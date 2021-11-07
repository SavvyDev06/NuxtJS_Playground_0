<template>
  <c-box bg="tan">
    <c-flex mx="20" my="0" justify="space-between" p="6">
      <c-flex>
        <c-text font-weight="bold" font-size="lg">DeGore</c-text>
      </c-flex>
      <c-flex>
        <c-text padding-right="10" font-size="lg">Menu 1</c-text>
        <c-text padding-right="10" font-size="lg">Menu 2</c-text>
        <c-text padding-right="10" font-size="lg">Menu 3</c-text>
        <c-text font-size="lg">Menu 4</c-text>
      </c-flex>
      <c-flex>
        <c-button variant="outline" color="gray.700" size="md"
          >Log out</c-button
        >
      </c-flex>
    </c-flex>
  </c-box>
</template>

<script>
import { CBox, CFlex, CText, CButton } from '@chakra-ui/vue'

export default {
  components: {
    CFlex,
    CText,
    CButton,
    CBox,
  },
}
</script>

<style></style>
