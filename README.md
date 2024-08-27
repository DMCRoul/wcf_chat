# WCF Chat Application

## Popis projektu

WCF Chat Application je distribuovaná aplikace pro výměnu zpráv v reálném čase postavená na technologii Windows Communication Foundation (WCF). Projekt se skládá ze tří hlavních částí:

1. **wcf_chat**: Obsahuje hlavní logiku chatu a implementaci WCF služby.
2. **ChatHost**: Hostingový server pro WCF službu.
3. **ChatClient**: Klientská aplikace pro komunikaci s WCF službou.

## Struktura projektu

### 1. wcf_chat

- **wcf_chat.csproj**: Projektový soubor pro knihovnu, která obsahuje hlavní logiku chatu a WCF službu.
- **app.config**: Konfigurační soubor pro nastavení WCF služby.
- **IServiceChat.cs**: Rozhraní služby, které obsahuje metody pro připojení, odpojení a odesílání zpráv v chatu.
- **ServerUser.cs**: Třída reprezentující uživatele chatu.
- **ServiceChat.cs**: Implementace WCF služby, která zpracovává připojení uživatelů, jejich odpojení a odesílání zpráv.

### 2. ChatHost

- **App.config**: Konfigurační soubor, který nastavuje hosting WCF služby pomocí HTTP a TCP protokolů.
- **Program.cs**: Hlavní vstupní bod pro spuštění hostingu WCF služby.

### 3. ChatClient

- **ChatClient.csproj**: Projektový soubor pro klientskou aplikaci.
- **App.config**: Konfigurační soubor pro připojení klienta k WCF službě.
- **MainWindow.xaml.cs**: Hlavní soubor obsahující logiku pro práci klientské aplikace, interakci s uživatelem a zpracování zpráv.

## Jak spustit projekt

### 1. Spuštění serveru

1. Otevřete projekt ChatHost.
2. Zkompilujte a spusťte projekt. Uvidíte zprávu Host se spustil!, což znamená úspěšné spuštění serveru.

### 2. Spuštění klienta

1. Otevřete projekt ChatClient.
2. Zkompilujte a spusťte projekt.
3. Zadejte uživatelské jméno a klikněte na Connect, abyste se připojili k chatu.

### 3. Použití chatu

- Zadejte zprávu do textového pole a stiskněte Enter pro odeslání zprávy.
- Zprávy se zobrazí v seznamu zpráv, který je přístupný všem připojeným uživatelům.

## Technologie

- **.NET Framework 4.8**: Pro vývoj aplikace.
- **WCF (Windows Communication Foundation)**: Pro vytvoření distribuované aplikace.
- **C#**: Hlavní programovací jazyk.


