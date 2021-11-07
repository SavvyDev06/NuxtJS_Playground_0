<template>
  <c-box>
    <c-text font-size="5xl" text-align="center" font-weight="bold"
      >Question 2</c-text
    >
    <c-text font-size="xl" text-align="center"
      >What is your level of experience?</c-text
    >
    <c-flex my="12" justify="center">
      <c-flex
        flex-direction="column"
        bg="indigo.200"
        mx="4"
        p="10"
        w="sm"
        rounded="lg"
        align="center"
      >
        <c-text mt="6" text-align="center" color="white" font-size="xl"
          >Beginner</c-text
        >
      </c-flex>
      <c-flex
        flex-direction="column"
        border-width="1px"
        mx="4"
        p="10"
        w="sm"
        rounded="lg"
        align="center"
      >
        <c-text mt="6" text-align="center" font-size="xl">Experienced</c-text>
      </c-flex>
      <c-flex
        flex-direction="column"
        border-width="1px"
        mx="4"
        p="10"
        w="sm"
        rounded="lg"
        align="center"
      >
        <c-text mt="6" text-align="center" font-size="xl">Professional</c-text>
      </c-flex>
    </c-flex>
    <c-flex justify="center">
      <c-button variant-color="indigo" bg="indigo.200" w="250px">Next</c-button>
    </c-flex>
    <c-box mx="auto" my="10" w="lg">
      <c-progress
        v-chakra="{
          div: {
            bg: 'indigo.200',
          },
        }"
        :value="60"
        height="40px"
        rounded="40px"
        has-stripe
        is-animated
      />
      <c-flex justify="space-between" my="3" mx="4">
        <c-text color="gray.700" font-size="sm">Step 2 Out of 5</c-text>
        <c-text color="gray.700" font-size="sm">60%</c-text>
      </c-flex>
    </c-box>
  </c-box>
</template>

<script>
import { CBox, CText, CFlex, CButton, CProgress } from '@chakra-ui/vue'

export default {
  components: {
    CBox,
    CText,
    CFlex,
    CButton,
    CProgress,
  },
}
</script>
