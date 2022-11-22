<script>
import { useRouter } from 'vue-router'
 
 export default {
    setup() {
        const router = useRouter()
        const click = () => {
            router.push({
                path: 'DashBoard'
            })
        }
        return {
            click
        }
    }
}
</script>

<template>
 
 <div class="container">
 <form action="" method="post">



 <label for="email">Email address</label>
 <input class="form-control" type="email" placeholder="@email.com" />
 <p>We'll never share your email with anyone else.</P>

 <label for="password">Password</label>
 <input class="form-control" type="password" placeholder="password" />

 <label for="password">Repeat Password</label>
 <input class="form-control" type="password" placeholder="password" />

 <button class="btn btn-primary mt-3" type="button" @click="click">Register</button>

 <p>Already have an account? <router-link to="/"  class="text-primary">Login</router-link> instead</P>



</form>
 </div>
</template>



<style>
body{
    margin-top: 0px;
    padding-top: 0px;
}
img{
    width:;
}
.reg{
    background-color:;
    color: white;
    border-radius: 3px;
    margin-botton: 20px;
    padding: 0px 5px 5px 5px;
}
label{
font-weight: bold;
color: ;
}
</style>