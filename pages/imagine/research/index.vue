<template>
  <div class="page imagine">
    <hero-section
      title="Research"
      subtitle="Methods for observation, information gathering, and testing"
      image="https://source.unsplash.com/zoCDWPuiRuA/1600x900"
      image-alt="Solution canvas, Amsterdam, Netherlands"
      color="primary"
      size="is-large"
    />
    <section-intro
      title="Forms of Research"
      subtitle="Research in the humanities involves different methods such as for example hermeneutics and semiotics. Humanities scholars usually do not search for the ultimate correct answer to a question, but instead, explore the issues and details that surround it. Context is always important, and context can be social, historical, political, cultural, or ethnic."
    >
      <p class="intro-paragraph">
        Research has been defined in a number of different ways, and while there
        are similarities, there does not appear to be a single, all-encompassing
        definition that is embraced by all who engage in it.
      </p>
      <p class="intro-paragraph">
        One definition of research is used by the OECD, “Any creative systematic
        activity undertaken in order to increase the stock of knowledge,
        including knowledge of man, culture and society, and the use of this
        knowledge to devise new applications.”
      </p>
      <a href="#design-thinking" id="design-thinking"><h2>Design Thinking is Grounded in Research</h2></a>
      <p>
        The theory and practice of design is evolving as technology changes and
        organizations adapt to a dynamic social, economic, political, and
        ecological environment.
      </p>
      <p>
        The role of the designer has been facing constant change as media and
        technology provide capabilities that had not been possible are quickly
        adopted by people who are trying to integrate the needs of people and
        business within the constraints of what is technically feasible.
      </p>
    </section-intro>
  </div>
</template>

<script>
import HeroSection from '~/components/HeroSection'
import SectionIntro from '~/components/SectionIntro'

export default {
  name: 'ImaginePage',
  components: {
    HeroSection,
    SectionIntro
  }
}
</script>
