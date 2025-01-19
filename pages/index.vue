<template>
  <div>
    <div class="columns mx-0 is-justify-content-center is-relative">
      <div class="column is-10">
        <div class="columns mx-0 mt-0">
          <div class="column mx-column py-4 bg-33335b border-r-12px mt-10px " v-for="(data, index) in select" :key="index">
            <div class="is-flex is-justify-content-space-between is-align-items-center">
              <div class="is-flex is-align-items-center">
                <img :src="data.img" alt="">
                <div class="mr-3">
                  <p class="color-33335b94 is-size-7">
                    {{ data.title }}
                  </p>
                  <p class="has-text-white is-size-6 font-bold-number">
                    {{ data.subtitle }}
                    <span class="is-size-7 has-text-white">
                      عدد
                    </span>
                  </p>
                </div>
              </div>
              <div>
                <img src="Chevron left.png" alt="">
              </div>
            </div>
          </div>
        </div>
        <div class="columns mx-0 my-0">
          <div class="column mx-column py-4 mt-10px bg-33335b has-text-centered border-r-12px" v-for="(data, index) in otherselect" :key="index">
            <div class="is-flex is-justify-content-space-between is-align-items-center">
              <div class="is-flex is-align-items-center">
                <img :src="data.img" alt="">
                <div class="mr-3">
                  <p class="color-33335b94 is-size-7">
                    {{ data.title }}
                  </p>
                  <p class="has-text-white is-size-6 font-bold-number">
                    {{ data.subtitle }}
                    <span class="is-size-7 has-text-white">
                      {{ data.span }}
                    </span>
                  </p>
                </div>
              </div>
              <div>
                <img src="Chevron left.png" alt="">
              </div>
            </div>
          </div>
        </div>
        <div class="columns mx-0 is-justify-content-center mt-5 ">
          <div class="column has-text-centered bg-33335b border-r-12px pt-5 pb-0">
            <div class="is-flex is-justify-content-space-between is-align-items-center mb-5">
              <div class="is-flex is-align-items-center">
                <p class="has-text-white font-bold-number">
                  تاریخچه تراکنش ها
                </p>
                <div class="field mb-0 mx-4">
                  <div class="control has-icons-left">
                    <input class="input bg-br-input is-size-7" type="text" placeholder="جستجو کنید...">
                    <span class="icon is-small is-left">
                      <img src="Search.png" alt="icon" class="pb-2">
                    </span>
                  </div>
                </div>
                <div class="is-flex w-170px py-1 is-align-items-center is-justify-content-space-between is-size-7">
                  <div class="is-flex is-align-items-center mr-2">
                    <img src="Calendar.png" alt="">
                    <p class="color-AEABD8">
                      10 آذر - 20 آبان
                    </p>
                  </div>
                  <div>
                    <img src="Vector 3.png" alt="" class="pl-2">
                  </div>
                </div>
              </div>
              <div class="is-flex is-align-items-center">
                <p class="is-size-7 color-33335b94">
                  تاریخچه تراکنش ها
                </p>
                <img src="Chevron left.png" alt="">
              </div>

            </div>
            <div class="columns is-mobile mb-1 mx-0">
              <div class="column color-AEABD8 is-size-7 is-1">
                ردیف
              </div>
              <div class="column color-AEABD8 is-size-7">
                نام و نام خانوادگی
              </div>
              <div class="column color-AEABD8 is-size-7">
                شماره کارت
              </div>
              <div class="column color-AEABD8 is-size-7">
                مبلغ
              </div>
              <div class="column color-AEABD8 is-size-7">
                تاریخ
              </div>
              <div class="column color-AEABD8 is-size-7">
                ساعت
              </div>
              <div class="column color-AEABD8 is-size-7 has-text-left">
                نام ترمینال
              </div>
            </div>
            <div class="columns mb-0 mx-0" v-for="(data, index) in ac_wd_etails" :key="index">
              <div class="column is-1">
                <img :src="data.counting" alt="">
              </div>
              <div class="column has-text-white is-size-7">
                {{ data.name }}
              </div>
              <div class="column has-text-white is-size-7">
                {{ data.cardnumber }}
              </div>
              <div class="column has-text-white is-size-7">
                {{ data.amount }} تومان
              </div>
              <div class="column has-text-white is-size-7">
                {{ data.date }}
              </div>
              <div class="column has-text-white is-size-7">
                {{ data.time }}
              </div>

              <div class="column has-text-grey is-size-7 is-flex  is-justify-content-end">
                <p class="w-65px color-AEABD8">
                  {{ data.terminal }}
                </p>
              </div>

            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      ac_wd_etails: [
        { counting: '1.png', name: 'پوریا احمدی', amount: '50,000', date: '12 آذر 1403', all: '100,000', cardnumber: '123456', time: '13:16', terminal: 'ایرانمال 1' },
        { counting: '2.png', name: 'پوریا احمدی', amount: '50,000', date: '12 آذر 1403', all: '100,000', cardnumber: '123456', time: '13:16', terminal: 'ایرانمال 2' },
        { counting: '3.png', name: 'پوریا احمدی', amount: '50,000', date: '12 آذر 1403', all: '100,000', cardnumber: '123456', time: '13:16', terminal: 'ایرانمال 3' },
        { counting: '4.png', name: 'پوریا احمدی', amount: '50,000', date: '12 آذر 1403', all: '100,000', cardnumber: '123456', time: '13:16', terminal: 'ایرانمال 4' },

      ],
      select: [
        { img: 'devices.png', title: 'تعداد دستگاه ها', subtitle: '34 ' },
        { img: 'Frame 2.png', title: 'تعداد تراکنش ها', subtitle: '1,532 ' },
      ],
      otherselect: [
        { img: 'cards.png', title: 'تعداد کارت ها', subtitle: '739', span: 'عدد' },
        { img: 'all mony.png', title: 'مجموع تراکنش ها', subtitle: '11,568,400', span: 'تومان' },
      ]
    }
  }
}
</script>