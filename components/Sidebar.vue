<template>
  <c-stack :spacing="5" width="20%">
    <c-box :p="2" shadow="md" border-width="1px">
      <c-flex justify="center">
        <c-button width="80%" margin="5px" border-width="1.6px"
          ><c-icon icon="user-secret" /><c-icon
            name="faEnvelope"
            size="24px"
            margin-right="2px"
          />Overview</c-button
        >
      </c-flex>
      <c-flex justify="center">
        <c-button width="80%" margin="5px" border-width="1.6px"
          >Configuration</c-button
        >
      </c-flex>
      <c-flex justify="center">
        <c-button width="80%" margin="5px" border-width="1.6px"
          >Settings</c-button
        >
      </c-flex>
      <c-flex justify="center">
        <c-button width="80%" margin="5px" border-width="1.6px"
          >Commands</c-button
        >
      </c-flex>
      <c-flex justify="center">
        <c-button width="80%" margin="5px" border-width="1.6px"
          >Action Logs</c-button
        >
      </c-flex>
      <c-flex justify="center">
        <c-button width="80%" margin="5px" border-width="1.6px"
          >DeGore Plus</c-button
        >
      </c-flex>
    </c-box>
  </c-stack>
</template>

<script>
import { CButton, CStack, CIcon } from '@chakra-ui/vue'

export default {
  components: {
    CButton,
    CStack,
    CIcon,
  },
}
</script>

<style></style>
