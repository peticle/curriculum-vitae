<script setup lang="ts">
import { BriefcaseBusiness } from "@lucide/vue";
import { DotList, DotListPeriod, SectionTitle } from "@/components";
</script>

<template>
  <section id="experience_professional">
    <SectionTitle>
      <template #icon><BriefcaseBusiness /></template>
      <h3>Expériences professionnelles</h3>
    </SectionTitle>
    <DotList>
      <DotListPeriod>
        <template #title>Service civil</template>
        <template #period>2025 &ndash; 2026</template>
        <template #subtitle>Porrentruy, Chevenez</template>
        <template #description>
          Aide-bibliothécaire à la Bibliothèque cantonale jurassienne et aide-éducateur à l'Unité
          d'accueil psycho-éducative.
        </template>
      </DotListPeriod>
      <DotListPeriod>
        <template #title>Développeur logiciel chez AZ Informatique</template>
        <template #period>2023 &ndash; 2025</template>
        <template #subtitle>Porrentruy</template>
        <template #description>
          Développement et maintenance de logiciels réalisés en Delphi 7 et 10, selon les demandes
          spécifiques ou les problèmes rencontrés par les clients. Conception, réalisation et
          gestion de projets pour des clients, consistant à développer des applications web conçues
          avec le framework Vue.js et le langage C#. Création de scripts, de services ou d'API web
          en C# et Python.
        </template>
      </DotListPeriod>
      <DotListPeriod>
        <template #title>Enseignement de cours de robotique</template>
        <template #period>2022 &ndash; 2023</template>
        <template #subtitle>Collège de Delémont</template>
        <template #description>
          Cours « Construire et programmer un robot » et « Les robots c'est l'affaire des filles »
          enseignés les samedis.
        </template>
      </DotListPeriod>
      <DotListPeriod>
        <template #title>Stage chez JAG Jakob SA</template>
        <template #period>2017 &ndash; 2018</template>
        <template #subtitle>Succursale de Porrentruy</template>
        <template #description>
          Stage réalisé dans le cadre de ma dernière année d'apprentissage. Celui-ci a
          majoritairement consisté à développer de nouvelles fonctionnalités pour les applications
          web de l'entreprise.
          <strong>Travail de diplôme :</strong>
          ajout dʼune interface interactive au système dʼhistorique dʼun module permettant la
          visualisation de lʼétat d'automates.
        </template>
      </DotListPeriod>
    </DotList>
  </section>
</template>
