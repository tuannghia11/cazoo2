<script>
/**
 * Register-2 component
 */
export default {
  head() {
    return {
      title: `Trang Đăng Ký`,
    };
  },
  data() {
    return {};
  },
  layout: "auth-2",
};
</script>

<template>
  <div>
    <!-- Logo -->
    <div class="auth-brand text-center text-lg-left">
      <div class="auth-logo">
        <nuxt-link to="/" class="logo logo-dark text-center">
          <span class="logo-lg">
            <img src="~/assets/images/logo-dark.png" alt height="22" />
          </span>
        </nuxt-link>

        <nuxt-link to="/" class="logo logo-light text-center">
          <span class="logo-lg">
            <img src="~/assets/images/logo-light.png" alt height="22" />
          </span>
        </nuxt-link>
      </div>
    </div>

    <!-- title-->
    <h4 class="mt-0">Đăng Ký</h4>
    <p class="text-muted mb-4">
      Bạn chưa có tài khoản? Chỉ cần chưa tới một phút để hoàn thành.
    </p>

    <form action="#">
      <div class="form-group">
        <label for="fullname">Họ và Tên</label>
        <input
          class="form-control"
          type="text"
          id="fullname"
          placeholder="Nhập tên của bạn"
          required
        />
      </div>
      <div class="form-group">
        <label for="emailaddress">Địa chỉ email</label>
        <input
          class="form-control"
          type="email"
          id="emailaddress"
          required
          placeholder="Nhập email của bạn"
        />
      </div>
      <div class="form-group">
        <label for="password">Mật khẩu</label>
        <div class="input-group input-group-merge">
          <input
            type="password"
            id="password"
            class="form-control"
            placeholder="Nhập mật khẩu của bạn"
          />
          <div class="input-group-append" data-password="false">
            <div class="input-group-text">
              <span class="password-eye"></span>
            </div>
          </div>
        </div>
      </div>
      
      </div>
      <div class="form-group mb-0 text-center">
        <button class="btn btn-primary btn-block" type="submit">Đăng ký</button>
      </div>
    <!-- Footer-->
    <footer class="footer footer-alt">
      <p class="text-muted">
        Đã có tài khoản?
        <nuxt-link to="/auth/register-2" class="text-primary ml-1">
          <b>Đăng nhập ngay!</b>
        </nuxt-link>
        <br />
        {{ new Date().getFullYear() }} &copy; Bản quyền thuộc
        <a href="http://keysoft.vn">Keysoft, inc</a>
      </p>
    </footer>
  </div>
</template>
