Unreal Engine Cache Manager Pro


📌 Visão Geral

O Unreal Engine Cache Manager Pro é uma ferramenta avançada para gerenciar e otimizar os arquivos de cache gerados pelo Unreal Engine. Ele ajuda desenvolvedores a:

    🗑️ Limpar caches de projetos individuais ou globais

    📊 Monitorar o uso de espaço em disco

    ⚙️ Configurar limpeza automática baseada em limites de espaço

    📈 Visualizar estatísticas de uso

✨ Recursos Principais
🔍 Gerenciamento de Projetos

    Escaneamento automático de projetos Unreal (.uproject)

    Configuração individual por projeto

    Limpeza seletiva de pastas (Intermediate, DerivedDataCache, Saved)

🌐 Cache Global

    Detecção automática de pastas de cache do sistema

    Gerenciamento do Unreal Engine Vault

    Adição de pastas de cache personalizadas

⏱ Monitoramento Automático

    Verificação periódica do espaço em disco

    Limpeza automática quando atingir limites configurados

    Configuração de intervalos de verificação

📊 Estatísticas

    Histórico de limpezas

    Uso de disco por partição

    Informações detalhadas do sistema

📥 Instalação
Requisitos

    Python 3.8+

    Unreal Engine 4.25+ (para projetos)

Método 1: Executável (Windows)

    Baixe o release mais recente

    Extraia o arquivo ZIP

    Execute UnrealCacheManager.exe

Método 2: Via Código Fonte
bash

git clone https://github.com/seu-usuario/unreal-cache-manager.git
cd unreal-cache-manager
pip install -r requirements.txt
python main.py

🛠 Configuração

Ao iniciar pela primeira vez, o programa irá:

    Criar um arquivo de configuração (unreal_cache_settings.json)

    Definir caminhos padrão para:

        Pasta de projetos

        Unreal Engine Vault

        Pastas de cache globais

Você pode ajustar essas configurações através da interface ou editando manualmente o arquivo.
🖥 Interface do Usuário
Aba "Projetos"

    Lista de todos os projetos Unreal encontrados

    Configurações individuais por projeto

    Ações rápidas (limpar, abrir pasta)

Aba "Unreal Vault"

    Informações sobre o tamanho do Vault

    Configurações de limpeza automática

    Gráfico de uso de espaço

Aba "Cache Global"

    Lista de todas as pastas de cache detectadas

    Opção para adicionar/remover pastas

    Limpeza seletiva

Aba "Estatísticas"

    Histórico de operações

    Informações do sistema

    Uso de disco

⚙️ Configurações Avançadas

O arquivo unreal_cache_settings.json permite ajustes avançados:
json

{
  "projects_path": "C:/Users/Usuario/Documents/Unreal Projects",
  "vault_path": "C:/Users/Usuario/AppData/Local/UnrealEngine/Common/DerivedDataCache",
  "global_cache_paths": [],
  "auto_monitor": false,
  "monitor_interval": 60,
  "start_with_windows": false,
  "start_minimized": false,
  "minimize_to_tray": true,
  "confirm_exit": true,
  "dark_mode": false,
  "check_updates": true
}

📜 Pastas Gerenciadas
Pastas Globais

    Windows:

        %LOCALAPPDATA%\UnrealEngine\Common\DerivedDataCache

        %LOCALAPPDATA%\UnrealEngine\Engine\DerivedDataCache

        %LOCALAPPDATA%\UnrealEngine\Engine\Intermediate

        %LOCALAPPDATA%\UnrealEngine\Engine\Saved\Logs

        %TEMP%\UnrealEngine

    Linux:

        ~/.cache/UnrealEngine/Common/DerivedDataCache

        ~/.local/share/UnrealEngine/Engine/Saved

    Mac:

        ~/Library/Application Support/Epic/UnrealEngine/Common/DerivedDataCache

        ~/Library/Application Support/Epic/UnrealEngine/Engine/DerivedDataCache

Pastas por Projeto

    Saved/

    Intermediate/

    DerivedDataCache/

⚠️ Avisos Importantes

    Sempre feche o Unreal Engine antes de limpar os caches

    A limpeza da pasta Saved/ pode remover configurações importantes

    Faça backup regular dos seus projetos

🤝 Contribuição

Contribuições são bem-vindas! Siga estes passos:

    Faça um fork do projeto

    Crie uma branch para sua feature (git checkout -b feature/AmazingFeature)

    Commit suas mudanças (git commit -m 'Add some AmazingFeature')

    Push para a branch (git push origin feature/AmazingFeature)

    Abra um Pull Request
