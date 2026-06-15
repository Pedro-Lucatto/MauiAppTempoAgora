# MauiAppTempoAgora

App feito em .NET MAUI que mostra o clima de qualquer cidade usando a API do OpenWeatherMap. Também usa a localização do dispositivo e exibe um mapa de ventos do Windy.

## O que faz

- Digita o nome da cidade e vê temperatura, sensação térmica, máxima, mínima, nascer/pôr do sol e ícone do clima
- Pega a localização atual pelo GPS e descobre a cidade automaticamente
- Mostra um mapa de ventos interativo embutido na tela

## Pra que plataforma

Android, iOS, macOS e Windows.

## Como usar

1. Pega uma chave grátis em https://openweathermap.org/api
2. Abre `Services/DataService.cs` e coloca a chave onde está `"insira-sua-chave"`
3. Roda com `dotnet build -t:Run -f net10.0-android` (ou troca o target pra iOS, Windows, etc)

## Estrutura

Services/DataService.cs   → chamada pra API
Models/Tempo.cs           → os dados do clima
MainPage.xaml/.cs         → tela principal e eventos
MauiProgram.cs            → startup
AppShell.xaml             → navegação

## Projeto feito com

- .NET 10 + MAUI
- Newtonsoft.Json
- OpenWeatherMap
- Windy (mapa embutido)
