scrip

<div class="flex items-center justify-center min-h-screen bg-gray-100">
  <div
    class="relative flex flex-col m-6 space-y-8 bg-white shadow-2xl rounded-2xl md:flex-row md:space-y-0"
  >

    <!-- left side -->
    <div class="relative bg-merva">
      <div class="w-[400px] h-full flex flex-col items-center justify-center space-y-2">
        <h1 class="font-serif text-center text-5xl text-white">MoneyToring</h1>
        <h1 class="font-bold text-center text-xl text-white">Pencatatan Keuangan Anda</h1>
      </div>
    </div>

    <!-- right side -->
    <div class="flex flex-col justify-center p-8 md:p-14">
      <span class="mb-3 text-4xl font-bold">Selamat datang!</span>
      <span class="font-light text-gray-500 mb-8">
        Silahkan login dengan akun yang diberikan oleh admin
      </span>
      <form action="/dashboard">
        <div class="py-4">
          <span class="mb-2 text-md">Email</span>
          <input
            type="text"
            class="w-full p-2 border border-gray-300 rounded-md placeholder:font-light placeholder:text-gray-500"
            name="email"
            id="email"
            required
          />
        </div>
        <div class="py-4">
          <span class="mb-2 text-md">Password</span>
          <input
            type="password"
            name="pass"
            id="pass"
            class="w-full p-2 border border-gray-300 rounded-md placeholder:font-light placeholder:text-gray-500"
            required
          />
        </div>
        <button
          class="w-full bg-merva text-white p-2 rounded-lg mb-6 hover:bg-white hover:text-black hover:border hover:border-gray-300" 
          type="submit"
          formaction="/app/dasbor"
        >
          Masuk
        </button>
        <div class="text-center text-gray-400">
          Ingin membuat akun atau lupa password?
          <a href="https://wa.me/6283185381334" target="_blank" class="font-bold text-merva">Klik disini!</a>
        </div>
      </form>
    </div>
    
  </div>
</div>