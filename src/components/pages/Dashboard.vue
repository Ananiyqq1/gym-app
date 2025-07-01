<script setup>
    import { gymHealthFacts } from '../../utils';
    import Grid from '../Grid.vue';

    const randomNumber = Math.floor(Math.random() * gymHealthFacts.length)
    const todayFact = gymHealthFacts[randomNumber]
</script>

<template>
<sction class="dashboard">
    <div class="card">
        <h2>Welcome Dear User</h2>
        <div class="tip-container">
            <p class="tip">
                <strong>Daily Tip</strong><br> {{ todayFact }} </p>
        </div>
        <button>Start Workout &rarr;</button>
    </div>
    <Grid />
</sction>
</template>

<style scoped>
.tip-container,
.tip-container div,
#dashboard{
 display: flex;   
}
.tip-container,
#dashboard{
    flex-direction: column;
}

#dashboard{
    gap: 0.5rem;
}

.tip-container{
    gap: 0.5rem;
}

@media (min-width: 640px){
    .tip-container{
        gap: 1rem;
    }
}


</style>