# nuachnichki

## **1. Клонирование репозитория**  
### **Windows / Linux**  
Откройте терминал (в Windows — `cmd` или PowerShell, в Linux — терминал) и выполните:  
```bash
git clone https://github.com/perin-nn/goydman_2025.git
cd goydman_2025
```

---

## **2. Установка Julia**  
### **Windows**  
1. Скачайте установщик с [официального сайта Julia](https://julialang.org/downloads/).  
2. Запустите `.exe` файл и следуйте инструкциям.  
3. Добавьте Julia в `PATH` (отметьте галочку при установке).  

### **Linux (Ubuntu/Debian)**  
```bash
sudo apt update
sudo apt install julia
```
Для других дистрибутивов используйте [официальные инструкции](https://julialang.org/downloads/platform/).

---

## **3. Установка пакетов Julia**  
Запустите Julia (`julia` в терминале) и выполните:  
```julia
using Pkg
Pkg.add([
    "BitInformation", "CodecZstd", "ColorSchemes", "FileIO", "JLD2",
    "LinLogQuantization", "NetCDF", "Plots", "PyCall", "PyPlot",
    "Statistics", "StatsBase", "TranscodingStreams", "ZfpCompression"
])
```

### **Дополнительные системные зависимости (Linux)**  
Для работы некоторых пакетов (`PyCall`, `NetCDF` и др.) могут потребоваться:  
```bash
sudo apt install python3 python3-pip libnetcdf-dev zstd
```
