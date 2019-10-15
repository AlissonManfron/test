## Mapeamento Analytics PJ iOS.


Este documento tem como finalidade mapear todas as classes que enviam algum tipo de Analytics para qualquer ferramenta, seja de terceiros ou interna.




## App Geral


# TermsOfUseViewController

  - TrackScreen: 
    - /Indices/Termos_de_Uso

  - Ferramentas:
    - Google Analytics
    - Firebase Analytics


# HomeViewCellServicos

  - TrackScreen: 
    - /Indices/Termos_de_Uso

  - TrackEvent: 
    - /Home/Chave
    - /Home/BIA
    - /Home/Pagamentos
    - /Home/TED
    - /Home/Pendentes
    - /Home/Recarga
    - /Home/Chave
    - /Home/Acesso a Conta

  - Ferramentas:
    - Google Analytics
    - Firebase Analytics


# ListAccountViewController

  - TrackScreen: 
    - /Sua_conta/Excluir_Conta
    - /Sua_conta/Editar_Conta

  - TrackEvent: 
    - SuaConta/AcessoAConta

  - Ferramentas:
    - Google Analytics
    - Firebase Analytics


# HomeViewCellBanners

  - TrackScreen: 

    - Open an external URL
      - /Apps/Home/abrir/externalUrl

    - Open an external App
      - /Apps/Home/abrir/urlScheme

    - Open an internal Area
      - /Apps/Home/abrir/data

    - Open an internal URL
      - /Apps/Home/abrir/data

  - TrackEvent: 
    
    - /Home/actionDataUnwrapped

    - Open an external URL
      - /Home/abrir/externalUrl

    - Open an external App
      - /Home/abrir/urlScheme

    - Open an internal Area
      - /Home/abrir/data

    - Open an internal URL
      - /Home/abrir/data

  - Ferramentas:
    - Google Analytics
    - Firebase Analytics




### Abertura de Contas MEI

  - TrackScreen: 
    - 

  - TrackEvent: 
    - 

  - Ferramentas:
    - Google Analytics
    - Firebase Analytics

### Atualização Cadastral 









