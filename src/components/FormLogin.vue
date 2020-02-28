<template>
    <div id="FormLogin">
        <form name="formLogin" id="formLogin" class="col-10 col-sm-6 col-md-4 col-lg-3 text-center child d-flex flex-column justify-content-center align-items-center">
            <div class="d-flex align-items-center mt-5">
                <img src="@/assets/img/lock.png" alt="">
            </div>
            <div class="form-row justify-content-center text-left my-4 w-100">
                <div class="col-md-12">
                    <label for="matricula" class="font-weight-bold text-blue">Matrícula</label>
                    <div class="input-group">
                        <input type="text" autocomplete="off" id="matricula" placeholder="" value="" required="required" class="form-control mx-auto" name="usuario" oninvalid="this.setCustomValidity('Preencha com a sua matricula.')" oninput="setCustomValidity('')">
                    </div>
                </div>
            </div>
            <div class="form-row justify-content-center text-left my-4 w-100">
                <div class="col-md-12">
                    <label for="password" class="font-weight-bold text-blue">Senha</label>
                    <input autocomplete="off" id="password" placeholder="" required="required" type="password" class="form-control mx-auto" name="senha" oninvalid="this.setCustomValidity('Preencha com a sua senha.')" oninput="setCustomValidity('')">
                </div>
            </div>
            <div class="form-group d-sm-flex mx-auto my-5 w-100">
                <button type="reset" class="btn btn-border-blue text-uppercase font-weight-bold text-blue w-100 mx-auto my-2">Limpar</button>
                <button type="submit" name="enviar" value="enviar" class="btn btn-blue text-white text-uppercase font-weight-bold w-100 mx-auto my-2">Acessar <i class="fa fa-arrow-circle-right"></i></button>
            </div>
        </form>
    </div>
</template>

<script>
export default {
    name: 'FormLogin'
}
</script>

<style>

</style>