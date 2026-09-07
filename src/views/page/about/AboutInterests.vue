<script setup lang="ts">
import { Gamepad2, Heart, Music, RectangleCircle, Server, UserGroup } from "@lucide/vue";
import { DotList, DotListItem, SectionTitle } from "@/components";
</script>

<template>
  <section id="about_interests">
    <SectionTitle>
      <template #icon><Heart /></template>
      <h3>Projets &amp; intérêts</h3>
    </SectionTitle>
    <DotList>
      <DotListItem>
        <template #left>
          <Server />
        </template>
        <template #right>
          Serveur personnel : virtualisation et hébergement de services (OPNsense, Proxmox, TrueNAS,
          Docker, Kubernetes).
        </template>
      </DotListItem>
      <DotListItem>
        <template #left>
          <RectangleCircle />
        </template>
        <template #right>
          Bibliothèque de composants Vue.js : conception et développement.
        </template>
      </DotListItem>
      <DotListItem>
        <template #left>
          <Music />
        </template>
        <template #right>
          Diffusion audio multi-pièce sur Raspberry Pi : streaming réseau synchronisé, sources
          analogiques et numériques.
        </template>
      </DotListItem>
      <DotListItem>
        <template #left>
          <Gamepad2 />
        </template>
        <template #right>
          Jeux vidéo : curiosité pour la conception et l'architecture des moteurs de jeu.
        </template>
      </DotListItem>
      <DotListItem>
        <template #left>
          <UserGroup />
        </template>
        <template #right>
          Jeunesse d'Alle : ancien membre du comité et membre actuel du comité d'organisation de la
          Rencontre des jeunesses jurassiennes 2027.
        </template>
      </DotListItem>
    </DotList>
  </section>
</template>

<style lang="scss" scoped>
#about_interests:deep(svg) {
  max-height: 1em;
  width: 1em;
}
</style>
