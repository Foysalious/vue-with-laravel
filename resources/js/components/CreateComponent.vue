<template>
  <div class="container">
    <div class="row justify-content-center">
      <div class="col-md-8">
        <div class="card">
          <div class="card-header">Create New Student</div>

          <div class="card-body">
            <form>
              <div class="form-group">
                <label for="exampleInputEmail1">Email address</label>
                <input
                  type="email"
                  v-model="email"
                  class="form-control"
                  id="exampleInputEmail1"
                  aria-describedby="emailHelp"
                  placeholder="Enter email"
                />
                <small id="emailHelp" class="form-text text-muted"
                  >We'll never share your email with anyone else.</small
                >
              </div>

               <div class="form-group">
                <label for="name">Name</label>
                <input
                  type="text"
                  v-model="name"
                  class="form-control"
                  id="name"
                  aria-describedby="emailHelp"
                  placeholder="Enter name"
                />
                
              </div>

              <div class="form-group">
                <label for="phone">Phone</label>
                <input
                  type="text"
                  v-model="phone"
                  class="form-control"
                  id="phone"
                  aria-describedby="emailHelp"
                  placeholder="Enter phone number"
                />
                
              </div>
              
              <button type="submit" class="btn btn-primary">Submit</button>
            </form>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
    data(){
        return {
            name:'',
            email:'',
            phone:''

        }
    },
  mounted() {
    console.log("Component mounted.");
  },
};
</script>
