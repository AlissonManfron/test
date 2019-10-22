
<h1 style="text-align:left;">
    Mapeamento Analytics PJ iOS.
    <span style="float:right; font-size: 14px;display: inline-block; line-height: 48px;">
        Atualizado em: 17/10/2019
    </span>
</h1>

Este documento tem como finalidade mapear todas as classes que enviam algum tipo de Analytics para qualquer ferramenta, seja de terceiros ou interna.


&nbsp;
&nbsp;
# App Geral


## TermsOfUseViewController

 #### TrackScreen: 

  - viewDidLoad()
    - /Indices/Termos_de_Uso

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## HomeViewCellServicos

#### TrackEvent: 

  - btnClicado(sender:)
    - /Home/Chave
    - /Home/BIA
    - /Home/Pagamentos
    - /Home/TED
    - /Home/Pendentes
    - /Home/Recarga

  - acessAccount(sender:)
    - /Home/Acesso a Conta

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## ListAccountsViewController

 #### TrackScreen: 

  - alertView()
    - /Sua_conta/Excluir_Conta
    - /Sua_conta/Editar_Conta

#### TrackEvent: 

  - tableView(_:didSelectRowAt:)
    - SuaConta/AcessoAConta

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## HomeViewCellBanners

 #### TrackScreen: 

  - itemPressed()
    - Open an external URL
      - /Apps/Home/abrir/$externalUrl

    - Open an external App
      - /Apps/Home/abrir/$urlScheme

    - Open an internal Area
      - /Apps/Home/abrir/$data

    - Open an internal URL
      - /Apps/Home/abrir/$data

#### TrackEvent: 
    
  - itemPressed()
    - /Home/$actionDataUnwrapped

    - Open an external URL
      - /Home/abrir/$externalUrl

    - Open an external App
      - /Home/abrir/$urlScheme

    - Open an internal Area
      - /Home/abrir/$data

    - Open an internal URL
      - /Home/abrir/$data

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## AccountWebViewController

 #### TrackScreen: 

  - webViewDidFinishLoad()
    - /Sua_conta/Primeiro_Acesso

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## SalvarChequeViewController

 #### TrackScreen: 

  - viewDidLoad()
    - /Deposito_Em_Cheque/Salvar_Cadastrar_Cheque

  - salvaChequeResultadoOK(sender:)
    - /Deposito_Em_Cheque/Cheque_Salvo

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## ApplicationsView

 #### TrackScreen: 

  - show()
    - /Apps

  - tableView(didSelectRowAt)
    - /Apps/Detalhe/$app.name

#### TrackEvent: 

  - productViewControllerDidFinish()
    - /Apps/instalar/Cancelada

  - tableView(didSelectRowAt)
    - /Apps/fechar/:$app.URI
    - /Apps/instalar/:$app.URI

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## FoneFacilViewController

 #### TrackScreen: 

  - tableView(didSelectRowAt)
    - /Ligar_Fone_Facil/Regioes_Metropolitanas
    - /Ligar_Fone_Facil/Demais_Localidades       
    - /Ligar_Fone_Facil/Acesso_do_Exterior"

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## BannersView

 #### TrackScreen: 

  - closeTouch(sender:)
    - /Apps/Home/fechar/:$url

#### TrackEvent: 

  - closeTouch(sender:)
    - /Apps/fechar/:$url

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## RightMenuViewController

#### TrackEvent: 

  - clickTermsInstitutionalMenu()
    - /Menu/Termos_Condicoes

  - clickSettingsInstitutionalMenu()
    - /Menu/Ajustes

  - clickUpdatePhotoProfile()
    - /Menu/Alterar_Foto_Perfil

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## Autorizador2DViewController

 #### TrackScreen: 

  - viewDidLoad()
    - /Token/Assinatura_Eletronica

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## TokenAtivacaoViewController

 #### TrackScreen: 

  - viewDidLoad()
    - /Token/Ativar

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## HomeViewController

 #### TrackScreen: 

  - viewWillAppear()
    - /Home

  - verificaAcessoViaWidget()
    - /Pendentes
    - /Pagamentos
    - /Saldo_e_Extrato    
    - /Transferencias

#### TrackEvent: 

  - callServiceNetwork()
    - /Menu/Rede_Atendimento

  - callBia()
    - /Menu/Bia

  - callSettings()
    - /Menu/Ajustes

  - callDailyEconomy()
    - /Menu/Economia_em_Dia

  - callUsefulphones()
    - /Menu/Telefones_Uteis

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## CameraChequeViewController

 #### TrackScreen: 

  - viewDidLoad()
    - /Deposito_Em_Cheque/Ajuste

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## OTPView

 #### TrackScreen: 

  - viewDidLoad()
    - /Token/Chave_de_Seguranca

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## BRATelemetria

#### TrackEvent: 

  - resume()
    - /WebViewFinishedTime/$label

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## PinLoginView

 #### TrackScreen: 

  - viewDidLoad()
    - /Token/Senha_Pessoal

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## PINConfigView

 #### TrackScreen: 

  - viewDidLoad()
    - /Token/Configurar_PIN

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## ViewControllerShortcutRouter

 #### TrackScreen: 

  - goToTransactionalViewControllerWithCampaign()
    - /Menu/Acesso_Conta

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## PerfilRenomearView 20

 #### TrackScreen: 

  - viewDidLoad()
    - /Token/Renomear_Chave

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## DailyEconomyViewController

 #### TrackScreen: 

  - showPDFTouch(sender:)
    - /Economia_Em_Dia/MaisRecentesDownloadPDF

  - dailyBoulletinTouch(sender:)
    - /Economia_Em_Dia/BoletimDiario

  - macroConjuctureTouch(sender:)
    - /Economia_Em_Dia/ConjunturaMacroEconomica

  - highlightExpress(sender:)
    - /Economia_Em_Dia/DestaqueExpresso

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## LeftMenuViewController

#### TrackEvent: 

  - clickHomeOnInstitutionalMenu()
    - /Menu/Inicio

  - clickBIAOnInstitutionalMenu()
    - /Menu/Bia

  - clickAccountAccessOnInstitutionalMenu()
    - /Menu/Acesso_Conta

  - clickAddCompanyOnInstitutionalMenu()
    - /Menu/Adicionar Empresa

  - clickSecurityKeyOnInstitutionalMenu()
    - /Menu/Token

  - clickDeposityCheckOnInstitutionalMenu()
    - /Menu/Deposito_Cheque

  - clickUsefulPhonesOnInstitutionalMenu()
    - /Menu/Telefones_Uteis

  - clickServiceNetworkOnInstitutionalMenu()
    - /Menu/Rede_Atendimento

  - clickDailyEconomyOnInstitutionalMenu()
    - /Menu/Economia_em_Dia

  - clickSteloMachineMenu()
     - /Menu/Contratacao_Stelo 

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## AccountAccessViewController

 #### TrackScreen: 

  - viewDidLoad()
    - /Sua_conta/Adicionar_Conta

#### TrackEvent: 

  - goesToBIA()
    - /Menu/Bia

  - setupAccountTableView()
    - /Sua_conta/Salvar_Certicado
    - /Sua_conta/Adicionar_Conta

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## BraChatViewController

 #### TrackScreen: 

  - viewWillAppear()
    - /Acesso_Bia

#### TrackEvent: 
  
  - goHome()
    - /Menu/Inicio

  - callUsefulphones()
    - /Menu/Telefones_Uteis

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## DailyEconomyFavoritesViewController

 #### TrackScreen: 

  - viewDidLoad()
    - /Economina_Em_Dia/Favoritos

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## CellphoneServicesViewController

 #### TrackScreen: 

  - webView(shouldStartLoadWith)
    - /Apps/ServicosCelular/abrir/$urlStr

#### TrackEvent: 

  - tableView(didSelectRowAt)
    - /SuaConta/AcessoAConta

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## AccountLoginViewController

 #### TrackScreen: 

  - webView(shouldStartLoadWith)
    - /Sua_conta/Acesso_a_Conta

#### TrackEvent: 

  - webViewDidFinishLoad()
    - /Sua_conta/PreencheuBoletodoPDF

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## LostAccessViewController

 #### TrackScreen: 

  - viewDidLoad()
    - /Sua_conta/Esqueci_Usuario
    - /Sua_conta/Perdi_Danifiquei_Acesso

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics 


## WelcomeAccountViewController

 #### TrackScreen: 

  - viewDidLoad()
    - /Sua_conta/Bem_Vindo

#### TrackEvent: 

  - showWalktrough()
    - /Sua_conta/Walkthrough

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## DailyEconomyHomeViewController

 #### TrackScreen: 

  - viewDidLoad()
    - /Economina_Em_Dia/Home

  - segmentedButtonAction()
    - /Economia_Em_Dia/Boletim_Diario_Matinal
    - /Economia_Em_Dia/Conjuntura
    - /Economia_Em_Dia/Destaque 

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


&nbsp;
&nbsp;
# Abertura de Contas MEI

## BRAPhotoViewController

 #### TrackScreen: 

  - viewDidAppear()
    - /mbpjaberturacontas/Captura_Documento
    - /mbpjaberturacontas/Captura_Documento

  - presentPerspectiveController()
    - /mbpjaberturacontas/AjustePerspectiva
    - /mbpjaberturacontas/AjustePerspectiva

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## BRAPhotoConfirmationViewController

 #### TrackScreen: 

  - viewDidAppear()
    - /mbpjaberturacontas/DocumentoAjustado

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## BRAInstructionsViewController

 #### TrackScreen: 

  - trackScreen()
    - /mbpjaberturacontas/InstrucoesNitidez
    - /mbpjaberturacontas/InstrucoesLuminosidade
    - /mbpjaberturacontas/ComprovanteEndereco
    - /mbpjaberturacontas/ComprovanteEnderecoEmpresa
    - /mbpjaberturacontas/ComprovanteDe6meses
    - /mbpjaberturacontas/InstrucoesContraste
    - /mbpjaberturacontas/InstrucoesComprovanteConta$documentType

  - configDocType()
    - /mbpjaberturacontas/InstrucoesVideoSelf

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## BRAModalAlertViewController

 #### TrackScreen: 

  - viewDidLoad()
    - /mbpjaberturacontas/PopupFalhaLer
    - /mbpjaberturacontas/PopupAjudaCaptura

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## BRATokenWebActivationViewController

 #### TrackScreen: 

  - viewDidAppear()
    - /mbpjaberturacontas/Pronto
    - /mbpjaberturacontas/ParabensContaAberta
    - /mbpjaberturacontas/InstrucoesAtivarToken

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## BRATokenWebActivationTermsViewController

 #### TrackScreen: 

  - viewDidAppear()
    - /mbpjaberturacontas/TermosToken

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## BRASelfieVideoDetailViewController

 #### TrackScreen: 

  - viewDidAppear()
    - /mbpjaberturacontas/QualidadeVideo

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## BRASelfieVideoViewController

 #### TrackScreen: 

  - viewDidAppear()
    - /mbpjaberturacontas/GravarVideoSelf

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## BRAOpenAccountWebViewController

 #### TrackScreen: 

  - jsCallNativeFunctions()
    - /mbpjaberturacontas/$tag_do_transacional

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## BRAWelcomeViewController

 #### TrackScreen: 

  - viewDidAppear()
    - /mbpjaberturacontas/BemVindo

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## BRAOpenAccountPassInfoController

 #### TrackScreen: 

  - viewDidAppear()
    - /mbpjaberturacontas/informacaoImportante

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## WebPinConfigView

 #### TrackScreen: 

  - viewDidLoad()
    - /mbpjaberturacontas/CadastroSenhaPIN

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


&nbsp;
&nbsp;
# Atualização Cadastral 
 

## SelectDocumentViewController

 #### TrackScreen: 

  - viewDidLoad()
    - /Atualizacao_CadastralPJ/Captura_Imagem_Endereco_Sede

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## DocumentDetailsViewController

 #### TrackScreen: 

  - viewDidAppear()
    - /Atualização_Cadastral_Pj/Captura_Faturamento/$documentType
    - /Atualização_Cadastral_Pj/Captura_Imagem_Endereco_Sede/$documentType

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## CaptureResultViewController

 #### TrackScreen: 

  - viewDidAppear()
    - /Atualização_Cadastral_Pj/Captura_Faturamento/Tela_Erro
    - /Atualização_Cadastral_Pj/Captura_Faturamento/Tela_Conclusao_Captura
    - /Atualização_Cadastral_Pj/Captura_Faturamento/Tela_Nova_Captura
    - /Atualização_Cadastral_Pj/Captura_Imagem_Endereco_Sede/Tela_Erro
    - /Atualização_Cadastral_Pj/Captura_Imagem_Endereco_Sede/Tela_Conclusao_Captura
    - /Atualização_Cadastral_Pj/Captura_Imagem_Endereco_Sede/Tela_Nova_Captura

#### TrackEvent: 

  - viewDidAppear()
    - /Atualização_Cadastral_Pj/FotosRestantes_$maxPages-currentPage

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## BRAPhotoViewController

 #### TrackScreen: 

  - viewDidAppear()
    - /Atualizacao_CadastralPJ/Captura_Faturamento/Captura_Documento
    - /Atualizacao_CadastralPJ/Captura_Imagem_Endereco_Sede/Captura_Documento

  - presentPerspectiveController()
    - /Atualizacao_CadastralPJ/Captura_Faturamento/AjustePerspectiva
    - /Atualizacao_CadastralPJ/Captura_Imagem_Endereco_Sede/AjustePerspectiva

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## BRAAddressTypeViewController

 #### TrackScreen: 

  - viewDidAppear()
    - /mbpjaberturacontas/SelecioneTipoComprovante

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics


## BRAPhotoConfirmationViewController

 #### TrackScreen: 

  - viewDidAppear()
    - /Atualizacao_CadastralPJ/Captura_Faturamento/DocumentoAjustado
    - /Atualizacao_CadastralPJ/Captura_Imagem_Endereco_Sede/DocumentoAjustado

#### Ferramentas:
  - Google Analytics
  - Firebase Analytics

# 
































