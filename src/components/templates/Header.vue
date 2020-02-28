<template>
    <header id="Header">
        <nav class="navbar navbar-expand-lg">
            <div class="col-md-4 text-center">
                <a class="navbar-brand m-0">
                <router-link to="/"><img class="navbar-brand img-fluid" src="@/assets/img/logo.png" alt="Relatório Justiça em Números"></router-link>
                </a>
            </div>
            <div class="col-md-4 p-0 justify-content-center align-content-center text-center">
                <a href="#" class="navbar-brand m-0">
                </a><h2 class="nav-link text-uppercase text-white font-weight-bold"><a href="#" class="navbar-brand m-0">
                </a><router-link to="/" class="text-white text-uppercase font-weight-bold">Relatório Justiça em Números</router-link>
                </h2>
            </div>
            <div class="col-md-4 justify-content-center align-content-center text-center">
                <button data-toggle="modal" data-target="#info-modal" class="btn btn-white nav-item text-uppercase font-weight-bold text-white">
                Saiba mais</button>
            </div>
        </nav>
        <div id="info-modal" tabindex="-1" role="dialog" aria-labelledby="info-modal-center-title" aria-hidden="true" class="modal fade">
            <div role="document" class="modal-dialog modal-dialog-centered modal-lg align-items-start">
                <div class="modal-content">
                <div class="modal-header bg-blue">
                    <h5 id="info-modal-title" class="modal-title text-white ml-auto pl-4">Ajuda</h5>
                    <button type="button" data-dismiss="modal" aria-label="Close" class="close text-white"><span aria-hidden="true">×</span></button>
                </div>
                <div class="modal-body text-left">
                    <p class="font-weight-bold">PARÂMETROS DE CONSULTA - CAMPOS:</p>
                    <p><span class="font-weight-bold">MATÉRIA:</span> É preciso selecionar o tipo da Matéria (Cível/Criminal)</p>
                    <p><span class="font-weight-bold">NUMERAÇÃO ÚNICA:</span> Somente Número</p>
                    <p>É necessário informar o número do processo até o ano da distribuição. Por exemplo: NNNNNNN-DD.AAAA.TR.0000, onde: NNNNNNN: Número do processo (sendo reiniciado a cada ano) DD: dígito verificador AAAA: ano do processo A consulta de processos criminais baixados ou em segredo de justiça é restrita apenas ao número do processo.</p>
                    <p><span class="font-weight-bold">NUMERO ANTIGO:</span> Somente Número</p>
                    <p><span class="font-weight-bold">PORTARIA IPM:</span> Informar o número do IPM ou APF, seguido do respectivo ano, com dois dígitos. Ex.: 123456/15</p>
                    <p><span class="font-weight-bold">NOME DA PARTE:</span> Livre</p>
                    <p>A consulta pelo nome da parte será realizada mesmo quando não for informado o nome completo, mas não retornará resultados de processos criminais baixados ou em segredo de justiça, cuja pesquisa é restrita ao número do processo.</p>
                    <p><span class="font-weight-bold">NÚMERO DO MILITAR:</span> Somente Número</p>
                    <p><span class="font-weight-bold">CPF DA PARTE:</span> Somente Número</p>
                    <p><span class="font-weight-bold">MADEP(MatrÍcula do Defensor Público):</span> Nesta pesquisa nao serão retornados processos eletrônicos.</p>
                    <p><span class="font-weight-bold">OAB do Advogado:</span> Somente Número</p>
                    <p><span class="font-weight-bold">NOME DA PARTE:</span> Livre</p>
                    <p>A consulta pelo CPF, Madep (número de matrícula do Defensor Público), número de OAB do advogado ou número do militar somente retornará resultados quando os dados forem informados de forma completa.</p>
                    Os critérios <span class="font-weight-bold">Contém</span> e <span class="font-weight-bold">Inicia com</span> só tem efeito para <span class="font-weight-bold">PARTES</span> ou <span class="font-weight-bold">ADVOGADOS</span> 
                    <p><span class="font-weight-bold">NUMERAÇÃO ÚNICA</span></p>
                    <p>É o número atribuído ao processo, que segue o padrão estabelecido pelo Conselho Nacional de justiça (CNJ), por meio da Resolução n. 65, de 16 de dezembro de 2008.</p>
                    <p><span class="font-weight-bold">PADRÃO DA NUMERAÇÃO ÚNICA</span></p>
                    <p>O padrão estabelecido pelo CNJ para a numeração única para os processos do Poder Judiciário é o seguinte: NNNNNNN-DD.AAAA.TR.0000, onde:</p>
                    <p><span class="font-weight-bold">NNNNNNN:</span> Número do processo ( sendo reiniciado a cada ano)</p>
                    <p><span class="font-weight-bold">DD:</span> dígito verificador</p>
                    <p><span class="font-weight-bold">AAAA:</span> ano do processo</p>
                    <p><span class="font-weight-bold">J:</span> Órgão do poder judiciário (no caso da Justiça Militar estadual, número 9)</p>
                    <p><span class="font-weight-bold">TR:</span> Identificação do tribunal (no caso da Justiça Militar de Minas Gerais, número 13) 0000: Código da unidade de origem (sendo OOO1 para a 1ª AJME, 00002 para a 2ª AJME, 0003 para a 3ª AJME e 0000 para o Tribunal de Justiça Militar de Minas Gerais). Assim, os números dos processos da Justiça Militar, dentro do padrão da numeração única, possuem a seguinte estrutura: NNNNNNNDDAAAA913000X (onde x é o código da origem podendo ser 0, 1, 2 ou 3).
                        Para consultar o andamento processual utilizando o número único, basta informar apenas os números correspondentes aos campos NNNNNNNDDAAAA, descritos acima.
                    </p>
                    <p><span class="font-weight-bold">NÚMERO ANTIGO</span></p>
                    Os processos distribuídos na Justiça Militar de Minas Gerais até 25 de Fevereiro de 2011 poderão ser consultados tanto pelo número antigo (número da Justiça Militar), quanto pelo número único padronizado pelo CNJ. Os processos distribuídos a partir de 28 de Fevereiro de 2011 deverão ser consultados somente pelo número único.
                    Estrutura do Número Antigo: 99999
                </div>
                </div>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    name: 'Header'
}
</script>

<style lang="scss">
    @media (max-width: 768px) {
        .navbar-nav {
            margin: auto !important;
        }
    }
</style>