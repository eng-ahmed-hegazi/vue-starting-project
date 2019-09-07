<template>
    <table class="table table-striped table-bordered">
        <tr>
            <th>No.</th>
            <th>Username</th>
            <th>Age</th>
            <th>Job</th>
            <th>Gender</th>
        </tr>
        <tr v-for="(person,index) in persons">
            <td>{{index+1}}</td>
            <td>{{person.name}}</td>
            <td>{{person.age}}</td>
            <td>{{person.job}}</td>
            <td>
                <span v-if="person.gender == 'female'">
                    <span class="label label-danger">Female</span>
                </span>
                <span v-if="person.gender == 'male'">
                    <span class="label label-primary">Male</span>
                </span>

            </td>
        </tr>
    </table>
</template>

<script>
    export default {
        data(){
            return{

            }
        }
    }
</script>
