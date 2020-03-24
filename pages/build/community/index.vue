<template>
  <div class="page build">
    <hero-section
      title="Community"
      subtitle="Social connection is the foundation for human identity"
      image="https://source.unsplash.com/W3SEyZODn8U/1600x900"
      image-alt="People eating a meal around a table"
      color="tertiary"
      size="is-large"
    />
    <section-intro
      title="Understanding Culture"
      subtitle="Humans acquire culture through the learning processes of enculturation and socialization, which is shown by the diversity of cultures across societies."
    >
      <p class="intro-paragraph">
        Humans acquire culture through the learning processes of enculturation and socialization, which is shown by the diversity of cultures across societies.
      </p>
      <a href="#social-connection" id="social-connection">
        <h2>Social connection is the foundation for human identity</h2>
      </a>
      <p>Culture (/ˈkʌltʃər/) is an umbrella term which encompasses the social behavior and norms found in human societies, as well as the knowledge, beliefs, arts, laws, customs, capabilities and habits of the individuals in these groups.</p>
      <p>Humans acquire culture through the learning processes of enculturation and socialization, which is shown by the diversity of cultures across societies.</p>
      <p>A cultural norm codifies acceptable conduct in society; it serves as a guideline for behavior, dress, language, and demeanor in a situation, which serves as a template for expectations in a social group. Accepting only a monoculture in a social group can bear risks, just as a single species can wither in the face of environmental change, for lack of functional responses to the change. Thus in military culture, valor is counted a typical behavior for an individual, as are duty, honor, and loyalty to the social group are counted as virtues or functional responses in the continuum of conflict. In the practice of religion, analogous attributes can be identified in a social group.</p>
      <p>Culture is considered a central concept in anthropology, encompassing the range of phenomena that are transmitted through social learning in human societies. Cultural universals are found in all human societies; these include expressive forms like art, music, dance, ritual, religion, and technologies like tool usage, cooking, shelter, and clothing. The concept of material culture covers the physical expressions of culture, such as technology, architecture and art, whereas the immaterial aspects of culture such as principles of social organization (including practices of political organization and social institutions), mythology, philosophy, literature (both written and oral), and science comprise the intangible cultural heritage of a society.</p>
      <ul>
        <li><a href="https://en.wikipedia.org/wiki/Culture" target="_blank">Wikipedia: Culture</a></li>
      </ul>
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
