<script setup>

</script>

<template>
    <section id="welcome">
        <div class="benefits">
            <h2>Upon Sucessful completion<br>You will achieve ...</h2>
            <div>
                <p>become more healthy, fit and shredded</p>
                <p>gurantee results with in 45 days</p>
            </div>
        </div>

        <div>
            <h3>Here's The Challenge</h3>
            <p>The Training Plan follows a structure known as the <strong>Bro Split</strong></p>
            <h5><i>Push &rarr; Pull &rarr; Legs &rarr; Repeat</i></h5>
        </div>

        <div class="card">
            <h3>Your Challenge</h3>
            <p>Complete all the workouts and track your progress along the way!</p>
            <p>Do you accept?</p>
            <button>Begin &rarr;</button>
        </div>

</section>
</template>

<style scoped>
    #welcome,
    .challenge,
    .benefits{
        display: flex;
        flex-direction: column;
    }
    #welcome{
        gap: 1.5rem;
    }
    .benefits{
        gap: 0.5rem;
    }
    .challenge{
        gap: 0.25rem;
    }
    @media(min-width: 640px) {
        #welcome{
            gap: 2rem;
            padding: 1rem 0;
        }
        .benefits{
            gap: 0.5rem;
        }
    }
</style>