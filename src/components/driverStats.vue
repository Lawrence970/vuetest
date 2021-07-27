<template>
    <div id="driverStats">
        <h2 class="large-text-h2">Routes of {{ currentDriver.first_name }} {{ currentDriver.last_name }}</h2>
        <span v-if="driverRoutes.length == 0">This Driver has no routes...</span>
        <span v-if="driverRoutes.length > 0">
            <ul>
                <li>
                    <h3>ID: {{route._id}}</h3>
                    <h3>FROM: {{route.from_location}}</h3>
                    <h3>TO: {{route.to_location}}</h3>
                    <h3>TOTAL: {{route.total_miles}} miles covered</h3>
                </li>
            </ul>
        </span>
    </div>
</template>

<script>
export default {

}
</script>

<style>

</style>