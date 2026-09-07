<script setup lang="ts">
import { StarCheck } from "@lucide/vue";
import { SectionTitle, SkillList, SkillListItem, SkillRating } from "@/components";
</script>

<template>
  <section id="experience_skills">
    <SectionTitle>
      <template #icon><StarCheck /></template>
      <h3>Compétences professionnelles</h3>
    </SectionTitle>
    <div id="experience_skills_lists">
      <section>
        <h4>Développement</h4>
        <SkillList>
          <SkillListItem>
            <template #left>HTML5 / CSS3</template>
            <template #right><SkillRating :rating="0.9" /></template>
          </SkillListItem>
          <SkillListItem>
            <template #left>SQL</template>
            <template #right><SkillRating :rating="0.8" /></template>
          </SkillListItem>
          <SkillListItem>
            <template #left>C#</template>
            <template #right><SkillRating :rating="0.7" /></template>
          </SkillListItem>
          <SkillListItem>
            <template #left>Python</template>
            <template #right><SkillRating :rating="0.7" /></template>
          </SkillListItem>
          <SkillListItem>
            <template #left>JS / TS</template>
            <template #right><SkillRating :rating="0.7" /></template>
          </SkillListItem>
          <SkillListItem>
            <template #left>C / C++</template>
            <template #right><SkillRating :rating="0.6" /></template>
          </SkillListItem>
        </SkillList>
      </section>
      <section>
        <h4>Outils développement</h4>
        <SkillList>
          <SkillListItem>
            <template #left>Git</template>
            <template #right><SkillRating :rating="0.7" /></template>
          </SkillListItem>
          <SkillListItem>
            <template #left>Docker</template>
            <template #right><SkillRating :rating="0.7" /></template>
          </SkillListItem>
          <SkillListItem>
            <template #left>Neovim</template>
            <template #right><SkillRating :rating="0.7" /></template>
          </SkillListItem>
          <SkillListItem>
            <template #left>Kubernetes</template>
            <template #right><SkillRating :rating="0.4" /></template>
          </SkillListItem>
        </SkillList>
      </section>
      <section>
        <h4>Logiciels</h4>
        <SkillList>
          <SkillListItem>
            <template #left>Suite Microsoft 365</template>
            <template #right><SkillRating :rating="0.8" /></template>
          </SkillListItem>
          <SkillListItem>
            <template #left>Photoshop / GIMP</template>
            <template #right><SkillRating :rating="0.6" /></template>
          </SkillListItem>
          <SkillListItem>
            <template #left>Inkscape</template>
            <template #right><SkillRating :rating="0.6" /></template>
          </SkillListItem>
          <SkillListItem>
            <template #left>Blender</template>
            <template #right><SkillRating :rating="0.3" /></template>
          </SkillListItem>
        </SkillList>
      </section>
      <section>
        <h4>Données / IA</h4>
        <SkillList>
          <SkillListItem>
            <template #left>Traitement d'images</template>
            <template #right><SkillRating :rating="0.7" /></template>
          </SkillListItem>
          <SkillListItem>
            <template #left>Traitement de données</template>
            <template #right><SkillRating :rating="0.6" /></template>
          </SkillListItem>
          <SkillListItem>
            <template #left>Machine learning</template>
            <template #right><SkillRating :rating="0.4" /></template>
          </SkillListItem>
        </SkillList>
      </section>
      <section>
        <h4>Infrastructure / Qualité</h4>
        <SkillList>
          <SkillListItem>
            <template #left>Réseau et systèmes</template>
            <template #right><SkillRating :rating="0.6" /></template>
          </SkillListItem>
          <SkillListItem>
            <template #left>Qualité logicielle</template>
            <template #right><SkillRating :rating="0.6" /></template>
          </SkillListItem>
          <SkillListItem>
            <template #left>Sécurité</template>
            <template #right><SkillRating :rating="0.5" /></template>
          </SkillListItem>
        </SkillList>
      </section>
    </div>
  </section>
</template>

<style lang="scss" scoped>
#experience_skills_lists {
  display: flex;
  flex-flow: column wrap;
  gap: 1rem;
  max-height: 380px;

  section {
    flex-grow: 1;

    ul {
      flex-grow: 1;
      gap: 0.2rem;
      justify-content: space-between;

      .skill-list-item:deep(.skill-rating) {
        border-color: var(--theme-clr-primary);

        .skill-rating_bar {
          background: var(--theme-clr-primary);
        }
      }
    }
  }
}
</style>
