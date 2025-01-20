<template>
    <div>
        <div class="columns mx-0 is-justify-content-center is-relative">
            <div class="column is-10">
                <div class="columns mx-0 mt-0">
                    <div class="column py-4 bg-33335b border-r-12px mt-10px ">
                        <div class="is-flex is-align-items-center">
                            <NuxtLink to="/">
                                داشبورد
                            </NuxtLink>
                            <img src="Chevron left.png" alt="" class="mx-1 w-15px" >
                            <p class="has-text-white font-bold-number">
                                ثبت تراکنش
                            </p>
                        </div>
                        <div class="px-3 py-3 w-350px mx-auto">
                            <div class="field mb-5">
                                <p class="is-size-7 color-AEABD8 mb-2">
                                    شماره کارت:
                                </p>
                                <div class="control has-icons-left">
                                    <input class="input bg-br-input is-size-7" type="text" placeholder="شماره کارت">
                                </div>
                            </div>
                            <div class="field mb-5">
                                <p class="is-size-7 color-AEABD8 mb-2">
                                    مبلغ:
                                </p>
                                <div class="control has-icons-left">
                                    <input class="input bg-br-input is-size-7" type="text" placeholder="0 تومان">
                                </div>
                            </div>
                            <div class="field mb-5">
                                <p class="is-size-7 color-AEABD8 mb-2">
                                    دستگاه:
                                </p>
                                <div class="control has-icons-left">
                                    <input class="input bg-br-input is-size-7" type="text" placeholder=" ...">
                                </div>
                            </div>
                            <button class="button w-100-bg-34C75945 is-size-7">
                                <div class="is-flex is-justify-content-center">
                                    ثبت
                                    <img src="Operation_ok.png" alt="" class="is-align-self-center mr-1" >
                                </div>
                                
                            </button>
                        </div>

                    </div>


                </div>
            </div>
        </div>
    </div>
</template>