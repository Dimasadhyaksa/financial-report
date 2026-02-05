<template>
  <Header />

  <div class="grid grid-cols-3 gap-6">
    <StatCard
      title="Operations"
      value="780"
      subtitle="/ 1000"
      :bars="8"
    />
    <StatCard
      title="Data Transfer"
      value="163"
      subtitle="/ 512.0 MB"
      :bars="6"
      highlight
    />
    <div class="bg-black rounded-2xl p-6 text-white flex flex-col justify-between">
      <p class="text-lg">
        Take Your Automation<br />
        to the Next Level
      </p>
      <button class="bg-white text-black px-4 py-2 rounded-xl w-fit">
        Upgrade
      </button>
    </div>
  </div>

  <ChartCard />
</template>
