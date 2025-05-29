# SupportTool: Ferramenta de Suporte Rápido

[![GitHub license](https://img.shields.io/badge/license-[SUA_LICENCA]-blue.svg)](LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/csousav98/SupportTool.svg?style=social)](https://github.com/csousav98/SupportTool/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/csousav98/SupportTool.svg?style=social)](https://github.com/csousav98/SupportTool/network/members)

Uma ferramenta de suporte desktop intuitiva, desenvolvida em C# e .NET Framework com **Windows Forms**, projetada para auxiliar técnicos e usuários finais com tarefas de diagnóstico e informações básicas do sistema.

## 🌟 Propósito e Motivação

Este projeto foi criado para fornecer uma interface rápida e fácil de usar para obter informações comuns do sistema, como endereços IP, versão do Windows e informações de rede. A intenção é simplificar o acesso a esses dados para fins de suporte técnico e solução de problemas.

## ✨ Funcionalidades Principais

* **Obter IP Público:** Exibe o endereço IP público do computador, obtido através de um serviço online.
* **Obter IP Interno:** Exibe o endereço IP interno do computador na rede local.
* **Obter Versão do Windows:** Exibe a versão do sistema operacional Windows instalado.
* **Obter Nome de Usuário Local:** Exibe o nome de usuário da conta local.
* **Obter Nome da Máquina Local:** Exibe o nome do computador.
* **Testar Ping:** Realiza um teste de ping para o IP interno e exibe o tempo de resposta, útil para verificar a conectividade da rede local.

## 🖥️ Screenshots

![Screenshot da Interface Principal](https://via.placeholder.com/600x400?text=Sua+Screenshot+Principal+Aqui)
*Substitua esta imagem por uma screenshot real da sua aplicação. É crucial mostrar a interface gráfica para que os usuários entendam como a ferramenta funciona.*

## 📋 Pré-requisitos

Para rodar esta aplicação a partir do código fonte, você precisará ter:

* **Visual Studio:** [Versão mínima recomendada, ex: Visual Studio 2019 ou superior]
* **.NET Framework SDK:** [Versão necessária, ex: .NET Framework 4.7.2 SDK ou superior]
* **Sistema Operacional:** Windows (aplicações Windows Forms são específicas para Windows).

## 🚀 Como Instalar e Rodar

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/csousav98/SupportTool.git](https://github.com/csousav98/SupportTool.git)
    cd SupportTool
    ```
2.  **Abra a solução no Visual Studio:**
    * Navegue até a pasta clonada e abra o arquivo `SupportTool.sln` com o Visual Studio.
3.  **Restaure os pacotes NuGet:**
    * No Visual Studio, vá em `Build > Restore NuGet Packages` ou clique com o botão direito na solução no Solution Explorer e selecione "Restore NuGet Packages".
4.  **Compile e execute:**
    * Pressione `F5` ou vá em `Debug > Start Debugging` para compilar e iniciar a aplicação.

## ⚙️ Configuração

A ferramenta utiliza o arquivo `App.config` para configurações internas do aplicativo. Este arquivo geralmente contém configurações de conexão ou outros parâmetros que podem ser ajustados. Edite este arquivo diretamente no Visual Studio.

## 📁 Estrutura do Projeto

```text
.
├── Images/                     # Recursos visuais (ícones, imagens)
│   ├── digital_globe11.ico
│   ├── digital_globe11.jpg
│   └── FR-Mitroff-Pervasive-Technology-1200x627-1200x627.jpg
├── SupportTool/                # Diretório principal do projeto C#
│   ├── bin/                    # Binários compilados (ignorados pelo Git)
│   │   └── Debug/
│   │       ├── SupportTool.exe
│   │       ├── SupportTool.exe.config
│   │       └── SupportTool.pdb
│   ├── obj/                    # Arquivos de build intermediários (ignorados pelo Git)
│   │   └── Debug/
│   │       ├── DesignTimeResolveAssemblyReferences.cache
│   │       ├── DesignTimeResolveAssemblyReferencesInput.cache
│   │       ├── SupportTool.csprojAssemblyReference.cache
│   │       ├── SupportTool.csproj.CoreCompileInputs.cache
│   │       ├── SupportTool.csproj.FileListAbsolute.txt
│   │       ├── SupportTool.csproj.GenerateResource.cache
│   │       ├── SupportTool.exe
│   │       ├── SupportTool.Form1.resources
│   │       ├── SupportTool.pdb
│   │       └── SupportTool.Properties.Resources.resources
│   ├── Properties/             # Propriedades do assembly e configurações do projeto
│   │   ├── AssemblyInfo.cs
│   │   ├── Resources.Designer.cs
│   │   ├── Resources.resx
│   │   ├── Settings.Designer.cs
│   │   └── Settings.settings
│   ├── App.config              # Configurações da aplicação (XML)
│   ├── Form1.cs                # Código da interface do usuário (Formulário principal)
│   ├── Form1.Designer.cs       # Código gerado automaticamente para o design do Formulário
│   ├── Form1.resx              # Recursos do Formulário (strings, imagens)
│   ├── Program.cs              # Ponto de entrada da aplicação
│   └── SupportTool.csproj      # Arquivo de projeto C#
└── SupportTool.sln             # Arquivo de solução do Visual Studio
├── README.md                   # Este arquivo README
└── LICENSE                     # Arquivo de licença do projeto (adicionar manualmente)
└── .gitignore                  # Arquivo para ignorar itens no Git (certifique-se de ignorar bin/, obj/, *.exe, *.pdb)
```

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** C#
* **Framework:** .NET Framework [Versão, ex: 4.7.2]
* **Interface Gráfica (GUI):** Windows Forms
* **Gerenciamento de Pacotes:** NuGet
* **Outras Bibliotecas:**
    * `System.Net`: Para obter o IP público.
    * `System.Management`: Para obter informações do sistema operacional.
    * `System.Net.NetworkInformation`: Para testar o ping.

## 🤝 Como Contribuir

Contribuições são bem-vindas! Se você tiver ideias, melhorias ou quiser corrigir bugs, por favor:

1.  Faça um fork do repositório.
2.  Crie uma nova branch para sua feature/correção (`git checkout -b feature/minha-nova-funcionalidade`).
3.  Faça suas alterações e adicione testes, se aplicável.
4.  Commit suas mudanças (`git commit -m 'feat: Adiciona Minha Nova Funcionalidade'`).
5.  Envie para sua branch (`git push origin feature/minha-nova-funcionalidade`).
6.  Abra um Pull Request, descrevendo suas mudanças.

## 📄 Licença

Este projeto está licenciado sob a Licença [Nome da sua licença, ex: MIT License] - veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 📧 Contato

Se você tiver dúvidas, sugestões ou precisar de suporte, sinta-se à vontade para abrir uma issue no GitHub ou entrar em contato em (https://www.linkedin.com/in/claudio-sousa-9b80a61a1/)

