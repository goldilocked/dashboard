<script setup lang="ts">
import type { NavigationMenuItem } from '@nuxt/ui'
import type { Member } from '~/types'

const links = [[{
  label: 'Members',
  icon: 'i-lucide-users',
  to: '/',
    children: [
      {
        label: "item 1",
      },
      {
        label: "item 2",
      },
      {
        label: "item 3",
      }
    ]
},{
  label: 'Members',
  icon: 'i-lucide-users',
  to: '/',
    children: [
      {
        label: "item 1",
      },
      {
        label: "item 2",
      },
      {
        label: "item 3",
      }
    ]
},{
  label: 'Members',
  icon: 'i-lucide-users',
  to: '/',
    children: [
      {
        label: "item 1",
      },
      {
        label: "item 2",
      },
      {
        label: "item 3",
      }
    ]
},{
  label: 'Members',
  icon: 'i-lucide-users',
  to: '/',
    children: [
      {
        label: "item 1",
      },
      {
        label: "item 2",
      },
      {
        label: "item 3",
      }
    ]
},{
  label: 'Members',
  icon: 'i-lucide-users',
  to: '/',
    children: [
      {
        label: "item 1",
      },
      {
        label: "item 2",
      },
      {
        label: "item 3",
      }
    ]
},{
  label: 'Members',
  icon: 'i-lucide-users',
  to: '/',
    children: [
      {
        label: "item 1",
      },
      {
        label: "item 2",
      },
      {
        label: "item 3",
      }
    ]
}]] satisfies NavigationMenuItem[][]
</script>

<template>
  <UDashboardPanel id="settings" :ui="{ body: 'lg:py-12' }">
    <template #header>
      <UDashboardNavbar title="Settings">
        <template #leading>
          <UDashboardSidebarCollapse />
        </template>
      </UDashboardNavbar>

      <UDashboardToolbar>
        <UNavigationMenu :items="links" class="flex-1" />
      </UDashboardToolbar>
    </template>

    <template #body>
      <div class="flex flex-col gap-4 sm:gap-6 lg:gap-12 w-full lg:max-w-2xl mx-auto">
  <div>
    <UPageCard
      title="Members"
      description="Invite new members by email address."
      variant="naked"
      orientation="horizontal"
      class="mb-4"
    >
    </UPageCard>

    <UPageCard variant="subtle" :ui="{ container: 'p-0 sm:p-0 gap-y-0', wrapper: 'items-stretch', header: 'p-4 mb-0 border-b border-default' }">

      <div>
        Some text to make this page seem less ridiculously empty.
      </div>
    </UPageCard>
  </div>      </div>
    </template>
  </UDashboardPanel>
</template>
