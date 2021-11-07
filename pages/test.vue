<template>
  <div>
    <c-button variant-color="indigo" @click="learnMoreToast"
      >Learn More</c-button
    >
    <c-button variant-color="green" @click="changesSavedToast"
      >Save Changes</c-button
    >
    <c-button variant-color="orange" @click="timedRevertableWarningToast"
      >Perform Dangerous Action</c-button
    >
    <c-button variant-color="red" @click="configDeletedToast"
      >Delete Configuration</c-button
    >
  </div>
</template>

<script lang="js">
import {
  CButton
} from '@chakra-ui/vue'

export default {
  name: 'App',
  components: {
    CButton
  },
  inject: ['$chakraColorMode', '$toggleColorMode'],
  data () {
    return {
      showModal: false,
      mainStyles: {
        dark: {
          bg: 'gray.700',
          color: 'whiteAlpha.900'
        },
        light: {
          bg: 'white',
          color: 'gray.900'
        }
      }
    }
  },
  computed: {
    colorMode () {
      return this.$chakraColorMode()
    },
    theme () {
      return this.$chakraTheme()
    },
    toggleColorMode () {
      return this.$toggleColorMode
    }
  },
  methods: {
    changesSavedToast () {
      this.$toast({
        title: 'Changes saved.',
        description: "We've successfully saved your changes.",
        status: 'success',
        duration: 6500,
        variant: 'subtle',
        position: 'top-right',
        isClosable: true
      })
    },
    timedRevertableWarningToast () {
        this.$toast({
            title: 'Heads up',
            description: 'You will not be able to revert this change 8 hours from now.',
            status: 'warning',
            duration: 10000,
            variant: 'solid',
            isClosable: false
        })
    },
    learnMoreToast () {
        this.$toast({
            title: 'More Info',
            description: `This is quite a cool website we've got going on here.`,
            status: 'info',
            duration: 15000,
            variant: 'solid',
            isClosable: true
        })
    },
    configDeletedToast () {
        this.$toast({
            title: 'Configuration Deleted.',
            description: `The configuration has been deleted.`,
            status: 'error',
            duration: 12000,
            variant: 'solid',
            position: 'top-right',
            isClosable: true
        })
    }
  }
}
</script>
