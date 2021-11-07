<template>
  <c-stack :spacing="5" width="20%">
    <c-box :p="2" shadow="md" border-width="1px">
      <c-flex justify="center">
        <c-button width="80%" margin="5px" border-width="1.6px">AI</c-button>
      </c-flex>
      <c-flex justify="center">
        <c-button width="80%" margin="5px" border-width="1.6px">AI</c-button>
      </c-flex>
      <c-flex justify="center">
        <c-button width="80%" margin="5px" border-width="1.6px">AI</c-button>
      </c-flex>
      <c-flex justify="center">
        <c-button width="80%" margin="5px" border-width="1.6px">AI</c-button>
      </c-flex>
      <c-flex justify="center">
        <c-button width="80%" margin="5px" border-width="1.6px">AI</c-button>
      </c-flex>
      <c-flex justify="center">
        <c-button width="80%" margin="5px" border-width="1.6px">AI</c-button>
      </c-flex>
    </c-box>
  </c-stack>
</template>

<script>
import { CButton, CStack } from '@chakra-ui/vue'

export default {
  components: {
    CButton,
    CStack,
  },
}
</script>

<style></style>
