<template>
  <div class="p-10">
    <h1 class="font-bold text-2xl mb-10">CRM system by Sokolov</h1>
    <div>
      <UiCard class="mb-3" draggable="true">
        <UiCardHeader role="button">name card</UiCardHeader>
        <UiCardContent>Компания</UiCardContent>
        <UiCardFooter>Date</UiCardFooter>
      </UiCard>
    </div>
  </div>
</template>

<script setup lang="ts">
import type {ICard, IColumn} from "~/components/kanban/kanban.types"
import {useKanbanQuery} from "@/components/kanban/useKanbanQuery";

useSeoMeta(
      {
        title: 'Home | CRM System',
      }
  )

  const dragCardRef = ref<ICard | null>(null)

  const sourceColumnRef = ref<IColumn | null>(null)

  useKanbanQuery()


</script>

<style lang="scss" scoped>

</style>