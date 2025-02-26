<!-- app.vue -->
<template>
  <div class="min-h-screen bg-gray-50">
    <div class="container mx-auto p-4">
      <h1 class="text-3xl font-bold mb-6 text-indigo-800">Nuxt 3 + Tailwind + PrimeVue Aura</h1>
      
      <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
        <div class="p-4 bg-white rounded-lg shadow">
          <h2 class="text-xl font-semibold mb-4">PrimeVue Components</h2>
          
          <PrimeCard class="mb-4">
            <template #title>PrimeVue Card</template>
            <template #content>
              <p>This is a PrimeVue Card component with the Aura theme.</p>
            </template>
            <template #footer>
              <PrimeButton label="Click Me" icon="pi pi-check" />
            </template>
          </PrimeCard>
          
          <div class="mb-4">
            <h3 class="mb-2">Button Examples:</h3>
            <Button label="Primary" class="mr-2" />
            <Button label="Secondary" severity="secondary" class="mr-2" />
            <Button label="Success" severity="success" class="mr-2" />
            <Button label="Warning" severity="warning" class="mr-2" />
            <Button label="Danger" severity="danger" />
          </div>
        </div>
        
        <div class="p-4 bg-white rounded-lg shadow">
          <h2 class="text-xl font-semibold mb-4">Tailwind Examples</h2>
          
          <div class="grid grid-cols-2 gap-4 mb-4">
            <div class="bg-blue-100 p-4 rounded">Tailwind Box 1</div>
            <div class="bg-purple-100 p-4 rounded">Tailwind Box 2</div>
            <div class="bg-green-100 p-4 rounded">Tailwind Box 3</div>
            <div class="bg-yellow-100 p-4 rounded">Tailwind Box 4</div>
          </div>
          
          <div class="bg-gradient-to-r from-indigo-500 to-purple-500 text-white p-6 rounded-lg">
            <h3 class="font-bold text-lg mb-2">Gradient Background</h3>
            <p>This uses Tailwind's gradient utilities.</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>