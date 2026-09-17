<script setup lang="ts">
import { BookText } from "@lucide/vue";
import { DotList, DotListPeriod, SectionTitle } from "@/components";
</script>

<template>
  <section id="about_studies">
    <SectionTitle>
      <template #icon><BookText /></template>
      <h3>Études et formation</h3>
    </SectionTitle>
    <DotList>
      <DotListPeriod>
        <template #title>Bachelor en Informatique &ndash; Ingénierie des données</template>
        <template #subtitle>Haute École Arc de Neuchâtel</template>
        <template #period>2020 &ndash; 2023</template>
        <template #description>
          <p>
            <strong>Travail intermédiaire pour Precitool SA : </strong>
            création d'un outil en Python pour extraire les mesures mathématiques de pièces
            réalisées avec Autodesk Inventor.
          </p>
          <p>
            <strong>Travail de bachelor pour Swiss Timing : </strong>
            création d'un système de stabilisation en temps réel du flux vidéo de caméras statiques,
            réalisé en Python avec OpenCV.
          </p>
        </template>
      </DotListPeriod>
      <DotListPeriod>
        <template #title>Maturité professionnelle technique</template>
        <template #subtitle> Division Technique du CEJEF de Porrentruy </template>
        <template #period>2018 &ndash; 2019</template>
      </DotListPeriod>
      <DotListPeriod>
        <template #title>CFC Informatique d'entreprise</template>
        <template #subtitle> Division Technique du CEJEF de Porrentruy </template>
        <template #period>2014 &ndash; 2018</template>
      </DotListPeriod>
    </DotList>
  </section>
</template>
