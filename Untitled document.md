**VONIX ROUTER**

1. Library

![](Aspose.Words.5108ed2b-2aa7-49a0-bd1a-0a3e6b072ee1.001.png)

Mengimport RouteRecordRaw, createWebHistory, dan createRouter dari Vue Router.

Mengimport View Home dari Home.vue.

Mengimport 6 komponen layout yang berbeda sebagai navigation di setiap halaman.

Mengimport useCookies dari library vue3-cookies.

Mengimport store dari Vuex.

Mengimport UserActionsType dari module user Vuex.

Mengimport UserMutationTypes dari module user Vuex.

1. Function

![](Aspose.Words.5108ed2b-2aa7-49a0-bd1a-0a3e6b072ee1.002.png)

Inisiasi Cookies dengan memasukkannya ke dalam variable cookies.

![](Aspose.Words.5108ed2b-2aa7-49a0-bd1a-0a3e6b072ee1.003.png)

Ketika membuka URL “/” akan memanggil view Home yang routenya diberi nama Home, dengan menggunakan LayoutSite sebagai navigationnya.

![](Aspose.Words.5108ed2b-2aa7-49a0-bd1a-0a3e6b072ee1.004.png)

Ketika membuka URL “/price” akan memanggil view Price dengan mengimport dari Price.vue. Price sebagai nama route dan component LayoutSite sebagai navigation.

![](Aspose.Words.5108ed2b-2aa7-49a0-bd1a-0a3e6b072ee1.005.png)

Ketika membuka URL “/customers” akan memanggil view Customers dengan mengimport dari Customers.vue. Customers sebagai nama route dan component LayoutSite sebagai navigation.

![](Aspose.Words.5108ed2b-2aa7-49a0-bd1a-0a3e6b072ee1.006.png)

Ketika membuka URL “/developers” akan memanggil view Developers dengan mengimport dari Developers.vue. Developers sebagai nama route dan component LayoutSite sebagai navigation.

![](Aspose.Words.5108ed2b-2aa7-49a0-bd1a-0a3e6b072ee1.007.png)

Ketika membuka URL “/company” akan memanggil view Company dengan mengimport dari Company.vue. Company sebagai nama route dan component LayoutSite sebagai navigation.

![](Aspose.Words.5108ed2b-2aa7-49a0-bd1a-0a3e6b072ee1.004.png)

Ketika membuka URL “/support” akan memanggil view SupportMain dengan mengimport dari SupportMain.vue. SupportMain sebagai nama route dan component LayoutSite sebagai navigation. Disini menggunakan teknik nested route, sehingga SupportMain mempunyai peran sebagai objek route induk dan memiliki properti children yang berisi objek route baru.

![](Aspose.Words.5108ed2b-2aa7-49a0-bd1a-0a3e6b072ee1.008.png)

Ketika membuka URL “/support” akan memanggil view Support dengan mengimport dari Support.vue yang merupakan child dari SupportMain. Support sebagai nama route dan layout navigation mengikuti induknya yang artinya menggunakan LayoutSite sebagai layout navigation.

![](Aspose.Words.5108ed2b-2aa7-49a0-bd1a-0a3e6b072ee1.007.png)

Ketika membuka URL “/support/:topic/topic” akan memanggil view TopicDetail dengan mengimport dari Topic.vue yang merupakan child dari SupportMain. TopicDetail sebagai nama route dan layout navigation mengikuti induknya yang artinya menggunakan LayoutSite sebagai layout navigation.

![](Aspose.Words.5108ed2b-2aa7-49a0-bd1a-0a3e6b072ee1.006.png)

Ketika membuka URL “/support/:question/question” akan memanggil view FaqDetail dengan mengimport dari Faq.vue yang merupakan child dari SupportMain. FadDetail sebagai nama route dan layout navigation mengikuti induknya yang artinya menggunakan LayoutSite sebagai layout navigation.

![](Aspose.Words.5108ed2b-2aa7-49a0-bd1a-0a3e6b072ee1.009.png)

Ketika membuka URL “/login” akan memanggil view Login dengan mengimport dari Login.vue. Login sebagai nama route dan component LayoutSiteLogin sebagai navigation. Memiliki variable OnlyGuest dengan type boolean yang mempunyai nilai true, artinya URL “/login” hanya bisa diakses oleh user yang belum login.

![](Aspose.Words.5108ed2b-2aa7-49a0-bd1a-0a3e6b072ee1.010.png)

Ketika membuka URL “/forgot-password” akan memanggil view ForgotPassword dengan mengimport dari ForgotPassword.vue. ForgotPassword sebagai nama route dan component LayoutSiteLogin sebagai navigation. Memiliki variable OnlyGuest dengan type boolean yang mempunyai nilai true, artinya URL “/forgot-password” hanya bisa diakses oleh user yang belum login.

![](Aspose.Words.5108ed2b-2aa7-49a0-bd1a-0a3e6b072ee1.011.png)

Ketika membuka URL “/reset-password” akan memanggil view ResetPassword dengan mengimport dari ResetPassword.vue. ResetPassword sebagai nama route dan component LayoutSiteLogin sebagai navigation. Memiliki variable OnlyGuest dengan type boolean yang mempunyai nilai true, artinya URL “/reset-password” hanya bisa diakses oleh user yang belum login.

![](Aspose.Words.5108ed2b-2aa7-49a0-bd1a-0a3e6b072ee1.006.png)

Ketika membuka URL “/register” akan memanggil view Register dengan mengimport dari Register.vue. Register sebagai nama route dan component LayoutSiteRegister sebagai navigation. Memiliki variable OnlyGuest dengan type boolean yang mempunyai nilai true, artinya URL “/register” hanya bisa diakses oleh user yang belum login.

![](Aspose.Words.5108ed2b-2aa7-49a0-bd1a-0a3e6b072ee1.012.png)

Ketika membuka URL “/email-verification-edit-profile” akan memanggil view EmailVerificationEditProfile dengan mengimport dari EmailVerificationEditProfile.vue. EmailVerificationEditProfile sebagai nama route dan component LayoutSiteRegister sebagai navigation.

![](Aspose.Words.5108ed2b-2aa7-49a0-bd1a-0a3e6b072ee1.009.png)

Ketika membuka URL “/about” akan memanggil view About dengan mengimport dari About.vue. About sebagai nama route dan component LayoutSite sebagai navigation.
