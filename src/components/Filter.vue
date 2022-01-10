<template>
    <div>
        <select v-model="selectValue" name="" id="">
            <option value="Rock">Rock</option>
            <option value="Jazz">Jazz</option>
            <option value="Cassic">Cassic</option>
        </select>
    </div>
</template>

<script>
export default {
    name: "Filter",
    data: function () {
        return {
            selectValue: ''
        };
    }
}
</script>