<template>
    <div id="Home">
        <div class="wrapper">
            <!-- Navbar -->
            <nav class="main-header navbar navbar-expand ">
                <div class="col-3 col-md-4 text-center">
                    <!-- Left navbar links -->
                    <ul class="navbar-nav">
                        <li class="nav-item">
                            <a class="nav-link" data-widget="pushmenu" href="#">
                            <img class="navbar-brand img-fluid" src="@/assets/img/open-menu.png" alt="Relatório Justiça em Números" width="24" height="24">
                            </a>
                        </li>
                    </ul>
                </div>
                <div class="col-7 col-md-4 text-center">
                    <a class="navbar-brand m-0">
                    <router-link to="/"><img class="navbar-brand img-fluid logo" src="@/assets/img/logo.png" alt="Relatório Justiça em Números"></router-link>
                    </a>
                </div>
                <div class="col-3 col-md-4 text-right">
                    <a class="navbar-brand m-0">
                    <router-link to="/"><img class="navbar-brand img-fluid user" src="@/assets/img/user.png" alt="Relatório Justiça em Números" width="40" height="40"></router-link>
                    </a>
                </div>
            </nav>
            <!-- /.navbar -->

            <!-- Main Sidebar Container -->
            <aside class="main-sidebar sidebar-dark-primary elevation-4">
                <!-- Brand Logo -->
                <a href="index3.html" class="brand-link text-center">
                <!-- <img src="@/assets/img/logo.png" alt="AdminLTE Logo" class="brand-image img-circle elevation-3"
                    style="opacity: .8"> -->
                <span class="text-white font-weight-bold text-uppercase">Relatório JN</span>
                </a>

                <!-- Sidebar -->
                <div class="sidebar">
                <!-- Sidebar user panel (optional) -->
                    <div class="user-panel mt-3 pb-3 mb-3 d-flex">
                        <div class="image">
                            <img class="img-circle elevation-2" src="@/assets/img/user.png" alt="Relatório Justiça em Números" width="40" height="40">
                        </div>
                        <div class="info">
                            <a href="#" class="d-block text-dark font-weight-bold text-uppercase">Alexander Pierce</a>
                        </div>
                    </div>

                    <!-- Sidebar Menu -->
                    <nav class="mt-2">
                        <ul class="nav nav-pills nav-sidebar flex-column" data-widget="treeview" role="menu" data-accordion="false">
                        <!-- Add icons to the links using the .nav-icon class
                            with font-awesome or any other icon font library -->
                        <li class="nav-item has-treeview menu-open">
                            <a href="#" class="nav-link active">
                            <i class="nav-icon fa fa-tachometer-alt"></i>
                            <p class="text-uppercase">
                                Starter Pages
                                <i class="right fa fa-angle-left"></i>
                            </p>
                            </a>
                            <ul class="nav nav-treeview">
                            <li class="nav-item">
                                <a href="#" class="nav-link active">
                                <i class="fa fa-circle nav-icon"></i>
                                <p  class="text-uppercase">Active Page</p>
                                </a>
                            </li>
                            <li class="nav-item">
                                <a href="#" class="nav-link">
                                <i class="fa fa-circle nav-icon"></i>
                                <p  class="text-uppercase">Inactive Page</p>
                                </a>
                            </li>
                            </ul>
                        </li>
                        <li class="nav-item">
                            <a href="#" class="nav-link">
                            <i class="nav-icon fa fa-th"></i>
                            <p  class="text-uppercase">
                                Simple Link
                                <span class="right badge badge-danger">New</span>
                            </p>
                            </a>
                        </li>
                        </ul>
                    </nav>
                
                <!-- /.sidebar-menu -->
                </div>
                <!-- /.sidebar -->
            </aside>

            <!-- Content Wrapper. Contains page content -->
            <div class="content-wrapper">

                <!-- Main content -->
                <div class="card w-75 mx-auto mt-5">
                    <div class="card-header bg-red pl-0">
                        <p class="text-white text-uppercase font-weight-bold pl-3 m-0">Tipo de Pesquisa</p>
                        <p class="border-bottom w-25 m-0"></p>
                    </div>
                    <div class="card-body">
                        <form name="formLogin" id="formLogin" class="col-md-8 col-lg-4 mx-auto mt-5">
                            <div class="form-group">
                                <label for="exampleFormControlInput1" class="text-blue text-uppercase font-weight-bold">Sistema</label>
                                <select class="form-control">
                                </select>
                            </div>
                            <div class="form-group">
                                <label for="exampleFormControlInput1" class="text-blue text-uppercase font-weight-bold">Tipo</label>
                                <select class="form-control">
                                </select>
                            </div>
                            <div class="form-group">
                                <label for="exampleFormControlInput1" class="text-blue text-uppercase font-weight-bold">Grupo(s)</label>
                                <select class="form-control">
                                </select>
                            </div>
                            <div class="form-group">
                                <label for="exampleFormControlInput1" class="text-blue text-uppercase font-weight-bold">Período</label>
                                <select class="form-control">
                                </select>
                            </div>
                                <label for="exampleFormControlInput1" class="text-blue text-uppercase font-weight-bold">Relatório</label>
                            <div id="d-flex">
                                <div class="form-check form-check-inline">
                                    <input class="form-check-input" type="radio" name="exampleRadios" id="exampleRadios1" value="option1">
                                    <label class="form-check-label text-blue" for="exampleRadios1">
                                        Relatório
                                    </label>
                                </div>
                                <div class="form-check form-check-inline ">
                                    <input class="form-check-input" type="radio" name="exampleRadios" id="exampleRadios2" value="option2">
                                    <label class="form-check-label text-blue" for="exampleRadios2">
                                        Analítico
                                    </label>
                                </div>
                            </div>
                                <label for="exampleFormControlInput2" class="text-blue text-uppercase font-weight-bold mt-3">Instância</label>
                            <div id="d-flex">
                                <div class="form-check form-check-inline">
                                    <input class="form-check-input" type="radio" name="exampleRadios" id="exampleRadios3" value="option3">
                                    <label class="form-check-label text-blue" for="exampleRadios3">
                                        1ª
                                    </label>
                                </div>
                                <div class="form-check form-check-inline">
                                    <input class="form-check-input" type="radio" name="exampleRadios" id="exampleRadios4" value="option4">
                                    <label class="form-check-label text-blue" for="exampleRadios4">
                                        2ª
                                    </label>
                                </div>
                            </div>
                            <div class="form-group d-sm-flex mx-auto my-3 w-100">
                                <button type="reset" class="btn btn-border-blue text-uppercase font-weight-bold text-blue w-100 mx-auto my-2">Visualizar <i class="fa fa-book"></i></button>
                                <button type="submit" name="enviar" value="enviar" class="btn btn-blue text-white text-uppercase font-weight-bold w-100 mx-auto my-2">Excel <i class="fa fa-download"></i></button>
                            </div>
                        </form>
                    </div>
                </div>
                <!-- /.content -->
            </div>
            <!-- /.content-wrapper -->


            <!-- Main Footer -->
            <footer class="main-footer">
                <!-- To the right -->
                <div class="float-right d-none d-sm-inline">
                Justiça Militar - 1ª e 2ª Instâncias
                </div>
                <!-- Default to the left -->
                <strong>Copyright &copy; 2014-2019 <a href="https://adminlte.io">AdminLTE.io</a>.</strong> All rights reserved.
            </footer>
        </div>
            <!-- ./wrapper -->
    </div>
</template>

<script>

export default {
    name: 'Home'
}
</script>

<style lang="scss">

@media (max-width: 576px) {
    .navbar-brand .logo{
        width: 174px;
    }
    .navbar-brand .user{
        width: 24px;
    }
    .main-header .col-9 {
        text-align: left !important;
    }
    .col-3 {
        -ms-flex: 0 0 25%;
        flex: 0 0 22% !important;
        max-width: 25%;
    }
}
</style>