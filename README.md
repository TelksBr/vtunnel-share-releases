<div align="center">

# 🌐 VTunnel Share Client — Releases Oficiais

[![Latest Pre-Release](https://img.shields.io/github/v/release/TelksBr/vtunnel-share-releases?include_prereleases&color=7C3AED&label=Pr%C3%A9-Release)](https://github.com/TelksBr/vtunnel-share-releases/releases)
[![Downloads](https://img.shields.io/github/downloads/TelksBr/vtunnel-share-releases/total?color=059669)](https://github.com/TelksBr/vtunnel-share-releases/releases)

**Cliente de tunelamento transparente para conexão via Hotspot SOCKS5 do app VTunnel.**  
Disponível para **Android** e **Windows (x64 e ARM64)**.

[📥 Baixar Última Versão](https://github.com/TelksBr/vtunnel-share-releases/releases/tag/v0.1.0-pre) • [📖 Como Usar](#-como-usar)

---
</div>

## 📥 Downloads Disponíveis (v0.1.0-pre)

### 📱 Android (7.0+)
| Arquitetura | Arquivo | Tamanho | Descrição |
| :--- | :--- | :--- | :--- |
| **ARM 64-bit** | [VTunnelShare-v0.1.0-arm64-v8a.apk](https://github.com/TelksBr/vtunnel-share-releases/releases/download/v0.1.0-pre/VTunnelShare-v0.1.0-arm64-v8a.apk) | 12.5 MB | Recomendado para 99% dos celulares modernos |
| **ARM 32-bit** | [VTunnelShare-v0.1.0-armeabi-v7a.apk](https://github.com/TelksBr/vtunnel-share-releases/releases/download/v0.1.0-pre/VTunnelShare-v0.1.0-armeabi-v7a.apk) | 12.1 MB | Para celulares mais antigos ou TV Box 32-bit |
| **Universal** | [VTunnelShare-v0.1.0-universal.apk](https://github.com/TelksBr/vtunnel-share-releases/releases/download/v0.1.0-pre/VTunnelShare-v0.1.0-universal.apk) | 22.9 MB | Pacote universal (todas as arquiteturas) |

### 💻 Windows (10/11)
| Arquitetura | Arquivo | Tamanho | Descrição |
| :--- | :--- | :--- | :--- |
| **Intel / AMD 64-bit (GUI)** | [VTunnelShare-v0.1.0-windows-amd64.exe](https://github.com/TelksBr/vtunnel-share-releases/releases/download/v0.1.0-pre/VTunnelShare-v0.1.0-windows-amd64.exe) | 12.0 MB | Interface gráfica de bandeja (Systray) para PCs x64 |
| **ARM 64-bit (GUI)** | [VTunnelShare-v0.1.0-windows-arm64.exe](https://github.com/TelksBr/vtunnel-share-releases/releases/download/v0.1.0-pre/VTunnelShare-v0.1.0-windows-arm64.exe) | 10.9 MB | Interface gráfica para Snapdragon X Elite / Surface Pro |
| **Intel / AMD 64-bit (CLI)** | [vtshare-cli-v0.1.0-windows-amd64.exe](https://github.com/TelksBr/vtunnel-share-releases/releases/download/v0.1.0-pre/vtshare-cli-v0.1.0-windows-amd64.exe) | 11.0 MB | Prompt de comando / automação para x64 |
| **ARM 64-bit (CLI)** | [vtshare-cli-v0.1.0-windows-arm64.exe](https://github.com/TelksBr/vtunnel-share-releases/releases/download/v0.1.0-pre/vtshare-cli-v0.1.0-windows-arm64.exe) | 9.9 MB | Prompt de comando / automação para ARM64 |

> ⚠️ **Aviso Windows:** Execute o aplicativo como **Administrador** para que o driver virtual Wintun possa criar a interface de rede TUN e configurar as rotas do sistema.

---

## 🚀 Como Usar

### 1. No Celular Servidor (VTunnel Principal)
1. Conecte sua VPN (SSH ou Xray/V2Ray).
2. Ligue o Roteador Wi-Fi (Hotspot) do celular.
3. Ative o **Compartilhar Conexão / Hotspot SOCKS5** no app VTunnel.
4. O app exibirá o IP e a Porta SOCKS5 (Ex.: `192.168.43.1:10808`).

### 2. No Dispositivo Cliente (Android ou Windows)
1. Conecte no Wi-Fi gerado pelo celular servidor.
2. Abra o **VTunnel Share Client**.
3. O app detectará o IP do Gateway automaticamente (ou informe manualmente).
4. Clique em **Conectar**.
5. Pronto! Todo o tráfego do sistema (TCP e UDP) estará navegando pelo túnel sem precisar de root.

---

## ✨ Recursos

- ⚡ **Roteamento Transparente:** Redireciona 100% das conexões do sistema sem necessidade de configurar proxy individual em cada app.
- 🎯 **Suporte Completo a UDP e TCP:** Compatível com Speedtest, jogos online, chamadas de áudio/vídeo (WhatsApp, Telegram) e DNS criptografado.
- 🛡️ **Zero Instalação Externa:** O driver de rede virtual (Wintun) já vem incorporado diretamente dentro do executável Windows.
- 🔋 **Leve e Otimizado:** Desenvolvido em Go (nativo) e Kotlin (nativo Android), garantindo estabilidade e baixo consumo.
