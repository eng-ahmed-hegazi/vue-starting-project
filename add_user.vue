<template>
    <div class="panel-heading">
        ADD NEW USER
    </div>
    <div class="panel-body">
        <div class="col-lg-11 ">
            <div class="form-group">
                <label for="name">Enter Username</label>
                <input type="text" id="name" placeholder="Enter Username" v-model="name" class="form-control">
            </div>
        </div>
        <div class="col-lg-11">
            <div class="form-group">
                <label for="age">Enter Age</label>
                <input type="text" id="age" placeholder="Enter Age" v-model="age" class="form-control">
            </div>
        </div>
        <div class="col-lg-11">
            <div class="form-group">
                <label for="job">Enter Job</label>
                <input type="text" id="job" placeholder="Enter Job" v-model="job" class="form-control">
            </div>
        </div>
        <div class="col-lg-11">
            <div class="form-group">
                <label for="gender">Select Gender</label>
                <select name="gender" id="gender" v-model="gender" class="form-control">
                    <option value="male">Male</option>
                    <option value="female">Female</option>
                </select>
            </div>
        </div>
        <div class="col-lg-11">
            <div class="form-group text-center">
                <button class="btn btn-primary" v-bind:disabled="disabledUser" @click="addNewUser">Add New User</button>
            </div>
        </div>

    </div>
</template>

<script>
    export default {
        data(){
            return{

            }
        }
    }
</script>
