<script setup>
import WelcomeItem from './WelcomeItem.vue'
import CultureIcon from './icons/IconCulture.vue'
import AdventureIcon from './icons/IconAdventure.vue'
import LandscapeIcon from './icons/IconLandscape.vue'
import SitesIcon from './icons/IconSites.vue'
import GastronomyIcon from './icons/IconGastronomy.vue'
</script>

<template>
  <WelcomeItem>
    <template #icon>
      <CultureIcon />
    </template>
    <template #heading>Cultural Immersion</template>

    Discover local traditions, cuisine, and customs, immersing yourself in the rich 
    cultural tapestry of each destination.
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <AdventureIcon />
    </template>
    <template #heading>Adventure Escapades</template>

    Embark on thrilling adventures, from hiking and safaris to water sports, 
    exploring the destination's natural wonders.
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <LandscapeIcon />
    </template>
    <template #heading>Scenic Landscapes</template>

    Unwind amidst stunning landscapes, from picturesque beaches and rolling 
    hills to majestic mountains and serene gardens.
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <SitesIcon />
    </template>
    <template #heading>Historical Marvels</template>

    Explore the historical wonders of each location, from ancient ruins and 
    temples to iconic landmarks that narrate captivating stories.
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <GastronomyIcon />
    </template>
    <template #heading>Gastronomic Delights</template>

    Savor local flavors and culinary delights, experiencing the unique taste 
    and essence of each destination's gastronomic offerings.
  </WelcomeItem>
</template>
