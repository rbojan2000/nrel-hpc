# NREL HPC

## O projektu
- Analiza podataka National Solar Radiation Database (NSRDB) - [NREL](https://nsrdb.nrel.gov/) Portorika za 2017. godinu.

- Redoslijed čitanja:
   1. [data_preparation.ipynb](notebooks/data_preparation.ipynb) Notebook
   2. [exploratory_analysis.ipynb](notebooks/exploratory_analysis.ipynb) Notebook
   3. [classification.ipynb](notebooks/classification.ipynb) Notebook
   4. [clusterization.ipynb](notebooks/clusterization.ipynb) Notebook

<br>

## Korišćene tehnologije
- **R**
- **Apache Arrow** - Čitanje Parquet fajlova
- **ggplot2** - Vizualizacija
- **caret** - Mašinsko učenje

<br>

## Pojmovi iz domena

1. **Solarni disk**  
   *Engl. solar disk*  
   - Predstavlja vidljivi dio Sunca na nebu. Površina Sunca koja emituje svjetlost.

2. **Iradijansa**  
   *Engl. irradiance*  
   - Fizička veličina koja označava snagu Sunčevog zračenja koja pada na jedinicu površine (izražava se u W/m²).  
   - Pokazuje koliko energije od Sunca dospijeva na površinu od 1 m² u određenom trenutku.

3. **Tipovi solarne iradijanse**  
   Sunčeva energija dospijeva do površine Zemlje na različite načine, pa razlikujemo tri osnovna tipa iradijanse:

   1. **Difuzna horizontalna iradijansa (DHI)**  
     *Engl. Diffuse Horizontal Irradiance*  
     - Dio Sunčevog zračenja koji je raspršen u atmosferi (oblaci, prašina, molekuli vazduha) i dolazi do površine iz svih pravaca, a ne direktno od Sunca.

   2. **Direktna normalna iradijansa (DNI)**  
     *Engl. Direct Normal Irradiance*  
      - Dio Sunčevog zračenja koji dolazi direktno od Solarnog diska, bez raspršivanja.
      - Mjeri se na površini koja je okomita (normalna) na Sunčeve zrake.

   3. **Globalna horizontalna iradijansa (GHI)**  
     *Engl. Global Horizontal Irradiance*  
      - Ukupna količina Sunčevog zračenja na horizontalnoj površini.  
      - Predstavlja zbir direktne i difuzne iradijanse:  
       GHI = DHI + DNI × cos(θ), gde je θ ugao između Sunčevih zraka i normale na površinu.