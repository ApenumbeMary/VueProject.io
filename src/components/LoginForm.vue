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
<div>
<form action="" method="post">

<h1 class="text-success">Kindly Login your imformations</h1>

<label>Email address</label><br> 
<input class="form-control" type="Email" placeholder=" @email.com" Required/>
<p class="">we'll not share your info with anyone.</P>

 
<label>password</label><br>
<input class="form-control" type="password" placeholder=" Enter password" Required/>


 <button class="btn btn-primary m-2" type="button" id="gettingstarted" @click="click">Login</button>

 <router-link to="/find-account" class="text-primary">ForgotPassword</router-link><br>
 
 

<span>New here?</span>
 <router-Link to="/reg" class="text-success" >Signup</router-Link>

</form>

</div>
</template>

<style>
.login{
    background-color: blue;
    color: white;
    border-radius: 5px;
    margin-right: 15px;
    padding: 0px 10px 3px 10px;
}
</style>