<template>
    <div class="full-page-center">
        <div class="form-container box bg-br-input ">
            
            <NuxtLink to="/" class="is-justify-content-center is-flex">
                <img src="logo.png" alt="">
                
            </NuxtLink >
            <div class="has-text-centered mt-3">
                <img src="user.png" alt="">
            </div>
            <form>
                <div class="field">
                    <label class="label color-AEABD8 ">ایمیل</label>
                    <div class="control">
                        <input class="input bg-br-input" type="email" placeholder="ایمیل خود را وارد کنید" />
                    </div>
                </div>
                <div class="field">
                    <label class="label color-AEABD8 ">رمز عبور</label>
                    <div class="control">
                        <input class="input bg-br-input" type="password" placeholder="رمز عبور خود را وارد کنید" />
                    </div>
                </div>
                <button class="button w-100-bg-34C75945 is-size-7">                     
                                    ثبت    
                            </button>
            </form>
        </div>
    </div>
</template>

<script>
export default {
    layout: "login",
};
</script>

<style scoped>
.full-page-center {
    display: flex;
    align-items: center;
    justify-content: center;
    min-height: 100vh;
}

.form-container {
    width: 100%;
    max-width: 400px;
    padding: 2rem;
    border-radius: 10px;
    box-shadow: 0px 0px 11px 0px rgb(255, 255, 255);
}
</style>