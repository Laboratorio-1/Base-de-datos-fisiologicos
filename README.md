DESCRIPCION GENERAL 


El conjunto de datos representado en la tabla proporciona información detallada sobre diferentes parámetros médicos y demográficos de varios sujetos, relacionados con un estudio médico de pacientes. Los datos que describe la tabla son:

Record #: Identificador único para cada registro en el conjunto de datos.

Age: La edad del sujeto, representada en años.

Gender: El género del sujeto, indicado por "M" para masculino y "F" para femenino.

Diagnosed: Indica si el sujeto ha sido diagnosticado con alguna condición médica, donde "y" representa sí y "n" representa no.

Treatment: Indica si el sujeto está recibiendo tratamiento médico, donde "y" representa sí y "n" representa no.

Systolic BP: La presión arterial sistólica del sujeto, medida en mmHg (milímetros de mercurio).

Diastolic BP: La presión arterial diastólica del sujeto, medida en mmHg.

Heart Rate: La frecuencia cardíaca del sujeto, medida en latidos por minuto (bpm).

JNC: Indica la clasificación de la presión arterial según las pautas del Comité Nacional Conjunto de EE. UU. sobre Prevención, Detección, Evaluación y Tratamiento de la Hipertensión (JNC). Las etiquetas pueden representar diferentes clasificaciones según la escala utilizada.

AHA: Indica la clasificación de la presión arterial según las pautas de la Asociación Americana del Corazón (AHA). Al igual que con JNC, las etiquetas pueden representar diferentes clasificaciones según la escala utilizada.


### BASE DE DATOS DE ESTIMACION ARTERIAL👋

</p>
        </section>
        
        <section id="acerca">
            <h2>ACERCA DE LA TABLA</h2>
            <p>La tabla consta de 11 columnas y 57 filas, representando cada fila un registro individual de cada sijeto debidamente identificado. Las columnas contienen detalles como edad, género, información sobre el diagnóstico médico de hipertensión, mediciones de presión arterial sistólica y diastólica, frecuencia cardíaca, estado de tratamiento, y una clasificación según los criterios de la Joint National Committee (JNC) y la Asociación Americana del Corazón (AHA) que determina si la persona es prehipertensa, normotensa o hipertensa. Cada registro está vinculado a un archivo separado por comas ".csv" de cada señal PPG que contiene los datos de medición específicos de ese individuo.</p>
        </section>
    </main>
        



<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Tabla de Información</title>
<style>
    table {
        width: 100%;
        border-collapse: collapse;
    }
    table, th, td {
        border: 1px solid black;
        padding: 8px;
        text-align: center;
    }
    th {
        background-color: #f2f2f2;
    }
</style>
</head>
<body>







<label for="ageFilter">Filtrar por edad:</label>
<select id="ageFilter">
    <option value="all">Todos</option>
    <option value="between40and50">Entre 40 y 50</option>
    <option value="between51and60">Entre 51 y 60</option>
    <option value="above60">Mayores de 60</option>
</select>

<label for="genderFilter">Filtrar por género:</label>
<select id="genderFilter">
    <option value="all">Todos</option>
    <option value="Masculino">Masculino</option>
    <option value="Femenino">Femenino</option>
</select>

<label for="jncFilter">Filtrar por JNC:</label>
<select id="jncFilter">
    <option value="all">Todos</option>
    <option value="Prehipertenso">Prehipertenso</option>
    <option value="Normotenso">Normotenso</option>
    <option value="Hipertenso">Hipertenso</option>
</select>

<label for="ahaFilter">Filtrar por AHA:</label>
<select id="ahaFilter">
    <option value="all">Todos</option>
    <option value="Prehipertenso">Prehipertenso</option>
    <option value="Normotenso">Normotenso</option>
    <option value="Hipertenso">Hipertenso</option>
</select>

<table id="data">
      <thead>
        <tr>
            <th>Sujeto</th>
            <th>Edad</th>
            <th>Género</th>
            <th>¿Está Diagnosticado?</th>
            <th>Presión Sitólica</th>
            <th>Presión Diastólica</th>
            <th>Frecuencia Cardiaca</th>
            <th>¿Está en Tratamiento?</th>
            <th>JNC</th>
            <th>AHA</th>
            <th>Archivos de la Señal PPG</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Sujeto 01</td>
            <td>44</td>
            <td>Masculino</td>
            <td>SI</td>
            <td>124</td>
            <td>83</td>
            <td>76</td>
            <td>NO</td>
            <td>Prehipertenso</td>
            <td>Hipertenso</td>
            <td><a href="https://drive.google.com/uc?export=download&id=1XwLobdcQq2OndmNc67r-G83ifQD63d5T" target="_blank">Signal_PPG_Subj_1</a></td>
        </tr>
        <tr>
            <td>Sujeto 02</td>
            <td>58</td>
            <td>Masculino</td>
            <td>SI</td>
            <td>115</td>
            <td>75</td>
            <td>84</td>
            <td>SI</td>
            <td>Normotenso</td>
            <td>Normotenso</td>
            <td><a href="https://drive.google.com/uc?export=download&id=1P5E85h_tk2rokxLIlfTuI2_2nfZ-OvLX" target="_blank">Signal_PPG_Subj_2</a></td>
        </tr>
        <tr>
            <td>Sujeto 03</td>
            <td>57</td>
            <td>Femenino</td>
            <td>SI</td>
            <td>121</td>
            <td>72</td>
            <td>56</td>
            <td>SI</td>
            <td>Prehipertenso</td>
            <td>Prehipertenso</td>
            <td><a href="https://drive.google.com/uc?export=download&id=1FPrYFA6ktLl7pWhm1UkBdiWe_4X_TbXd" target="_blank">Signal_PPG_Subj_3</a></td>
        </tr>

</tr>
<tr>
    <td>Sujeto 04</td>
    <td>48</td>
    <td>Femenino</td>
    <td>SI</td>
    <td>125</td>
    <td>75</td>
    <td>73</td>
    <td>SI</td>
    <td>Prehipertenso</td>
    <td>Prehipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1Dsb0ad1JQ2COKa0FeRMJf4fBfyGcyzIi" target="_blank">Signal_PPG_Subj_4</a></td>
</tr>

<tr>
    <td>Sujeto 05</td>
    <td>46</td>
    <td>Femenino</td>
    <td>SI</td>
    <td>97</td>
    <td>64</td>
    <td>86</td>
    <td>SI</td>
    <td>Normotenso</td>
    <td>Normotenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1yUknSAD5gkhtBcDLO8yR1RItbokD0KRS" target="_blank">Signal_PPG_Subj_5</a></td>
</tr>

<tr>
    <td>Sujeto 06</td>
    <td>65</td>
    <td>Femenino</td>
    <td>SI</td>
    <td>119</td>
    <td>57</td>
    <td>85</td>
    <td>SI</td>
    <td>Normotenso</td>
    <td>Normotenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1uCnNpBFij1wWV3pOMhZc73fcXZAYsZc8" target="_blank">Signal_PPG_Subj_6</a></td>
</tr>


<tr>
    <td>Sujeto 07</td>
    <td>60</td>
    <td>Femenino</td>
    <td>SI</td>
    <td>161</td>
    <td>94</td>
    <td>68</td>
    <td>SI</td>
    <td>Hipertenso</td>
    <td>Hipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=10ORVrVfRv5u0uA97UEPGSTqBclapfZvw" target="_blank">Signal_PPG_Subj_7</a></td>
</tr>

<tr>
    <td>Sujeto 08</td>
    <td>47</td>
    <td>Masculino</td>
    <td>SI</td>
    <td>148</td>
    <td>96</td>
    <td>58</td>
    <td>NO</td>
    <td>Hipertenso</td>
    <td>Hipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1M_6YzQg7BBh4h-9t3qASn48CHvaK4Tso" target="_blank">Signal_PPG_Subj_8</a></td>
</tr>
<tr>
    <td>Sujeto 09</td>
    <td>46</td>
    <td>Femenino</td>
    <td>SI</td>
    <td>122</td>
    <td>74</td>
    <td>62</td>
    <td>SI</td>
    <td>Prehipertenso</td>
    <td>Prehipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1Nwof9mm2RehVR20c98s0tHW7bT_JJKd8" target="_blank">Signal_PPG_Subj_9</a></td>
</tr>
<tr>
    <td>Sujeto 10</td>
    <td>58</td>
    <td>Femenino</td>
    <td>SI</td>
    <td>114</td>
    <td>71</td>
    <td>75</td>
    <td>SI</td>
    <td>Normotenso</td>
    <td>Normotenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1qUqKUMnvGmS3b2Swn3bw3n7RAwdhmVYe" target="_blank">Signal_PPG_Subj_10</a></td>
</tr>
<tr>
    <td>Sujeto 11</td>
    <td>57</td>
    <td>Masculino</td>
    <td>SI</td>
    <td>112</td>
    <td>72</td>
    <td>75</td>
    <td>SI</td>
    <td>Normotenso</td>
    <td>Normotenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1sRO5CCQREs1eKQ3S8sfELkPj4f4GmLzA" target="_blank">Signal_PPG_Subj_11</a></td>
</tr>
<tr>
    <td>Sujeto 12</td>
    <td>65</td>
    <td>Masculino</td>
    <td>SI</td>
    <td>111</td>
    <td>70</td>
    <td>75</td>
    <td>NO</td>
    <td>Normotenso</td>
    <td>Normotenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1xCVQgqpepXVZdYJKVqjJ1QgXxyYp6MZZ" target="_blank">Signal_PPG_Subj_12</a></td>
</tr>
<tr>
    <td>Sujeto 13</td>
    <td>45</td>
    <td>Femenino</td>
    <td>NO</td>
    <td>144</td>
    <td>87</td>
    <td>65</td>
    <td>NO</td>
    <td>Hipertenso</td>
    <td>Hipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1coqioEic_P0JUy67HHcnTNWMe5OgbZls" target="_blank">Signal_PPG_Subj_13</a></td>
</tr>
<tr>
    <td>Sujeto 14</td>
    <td>45</td>
    <td>Femenino</td>
    <td>NO</td>
    <td>130</td>
    <td>90</td>
    <td>88</td>
    <td>NO</td>
    <td>Hipertenso</td>
    <td>Hipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1moE_bjxJmcSfIol2amDDtIZnGpklS-OR" target="_blank">Signal_PPG_Subj_14</a></td>
</tr>
<tr>
    <td>Sujeto 15</td>
    <td>45</td>
    <td>Femenino</td>
    <td>NO</td>
    <td>103</td>
    <td>65</td>
    <td>97</td>
    <td>NO</td>
    <td>Normotenso</td>
    <td>Normotenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1Rj_39qlIuE49jVcPYn6RQil_3M3EBVvY" target="_blank">Signal_PPG_Subj_15</a></td>
</tr>
<tr>
    <td>Sujeto 16</td>
    <td>48</td>
    <td>Femenino</td>
    <td>SI</td>
    <td>152</td>
    <td>109</td>
    <td>100</td>
    <td>NO</td>
    <td>Hipertenso</td>
    <td>Hipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1ovUsFC-RfOLqDDkUmCp8rlmabN_jJxIR" target="_blank">Signal_PPG_Subj_16</a></td>
</tr>
<tr>
    <td>Sujeto 17</td>
    <td>65</td>
    <td>Femenino</td>
    <td>NO</td>
    <td>133</td>
    <td>81</td>
    <td>77</td>
    <td>NO</td>
    <td>Prehipertenso</td>
    <td>Hipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1kJg2tcjy4u_NjxY5LFgHieKYkV8HE2xO" target="_blank">Signal_PPG_Subj_17</a></td>
</tr>
<tr>
    <td>Sujeto 18</td>
    <td>45</td>
    <td>Femenino</td>
    <td>NO</td>
    <td>135</td>
    <td>90</td>
    <td>84</td>
    <td>NO</td>
    <td>Hipertenso</td>
    <td>Hipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1pdpuAL7DXv0FXQwS9MXr5FWTLH6kHXLx" target="_blank">Signal_PPG_Subj_18</a></td>
</tr>
<tr>
    <td>Sujeto 19</td>
    <td>57</td>
    <td>Femenino</td>
    <td>NO</td>
    <td>120</td>
    <td>68</td>
    <td>58</td>
    <td>NO</td>
    <td>Normotenso</td>
    <td>Prehipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1Jpx5if1cT8RbdBF7Igf_Crt4_Urn39sX" target="_blank">Signal_PPG_Subj_19</a></td>
</tr>
<tr>
    <td>Sujeto 20</td>
    <td>53</td>
    <td>Femenino</td>
    <td>SI</td>
    <td>154</td>
    <td>93</td>
    <td>62</td>
    <td>NO</td>
    <td>Hipertenso</td>
    <td>Hipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1J9bL5GliOF7N2vcVY1ICf3J0jTF3yWTh" target="_blank">Signal_PPG_Subj_20</a></td>
</tr>
<tr>
    <td>Sujeto 21</td>
    <td>55</td>
    <td>Femenino</td>
    <td>NO</td>
    <td>125</td>
    <td>84</td>
    <td>62</td>
    <td>NO</td>
    <td>Prehipertenso</td>
    <td>Hipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1E_p2wzZAsqVKUNepFn0hR3Y5iLYB6JxR" target="_blank">Signal_PPG_Subj_21</a></td>
</tr>
<tr>
    <td>Sujeto 22</td>
    <td>45</td>
    <td>Femenino</td>
    <td>NO</td>
    <td>106</td>
    <td>60</td>
    <td>53</td>
    <td>NO</td>
    <td>Normotenso</td>
    <td>Normotenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1C4CM-XyyQV4XStG1JewjZh0gD-5M_q1b" target="_blank">Signal_PPG_Subj_22</a></td>
</tr>
<tr>
    <td>Sujeto 23</td>
    <td>45</td>
    <td>Masculino</td>
    <td>SI</td>
    <td>127</td>
    <td>82</td>
    <td>71</td>
    <td>SI</td>
    <td>Prehipertenso</td>
    <td>Hipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1Kfh-KyJVgXlXyiw_XO-f15zAxlYj2EEh" target="_blank">Signal_PPG_Subj_23</a></td>
</tr>
<tr>
    <td>Sujeto 24</td>
    <td>57</td>
    <td>Femenino</td>
    <td>SI</td>
    <td>110</td>
    <td>60</td>
    <td>78</td>
    <td>SI</td>
    <td>Normotenso</td>
    <td>Normotenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1h7aK4d7x36-Gn9okQLtyGFdyzYwhh5mL" target="_blank">Signal_PPG_Subj_24</a></td>
</tr>
<tr>
    <td>Sujeto 25</td>
    <td>45</td>
    <td>Femenino</td>
    <td>NO</td>
    <td>115</td>
    <td>60</td>
    <td>72</td>
    <td>NO</td>
    <td>Normotenso</td>
    <td>Normotenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1OwAvdPzW_1sX7q9uEEwVXZtnRcMw7p6I" target="_blank">Signal_PPG_Subj_25</a></td>
</tr>
<tr>
    <td>Sujeto 26</td>
    <td>45</td>
    <td>Femenino</td>
    <td>SI</td>
    <td>137</td>
    <td>90</td>
    <td>69</td>
    <td>SI</td>
    <td>Hipertenso</td>
    <td>Hipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1qE6AQ1-Rv46_bOiawVvXyJJWWHsP4wqY" target="_blank">Signal_PPG_Subj_26</a></td>
</tr>
<tr>
    <td>Sujeto 27</td>
    <td>56</td>
    <td>Femenino</td>
    <td>NO</td>
    <td>135</td>
    <td>97</td>
    <td>69</td>
    <td>NO</td>
    <td>Hipertenso</td>
    <td>Hipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1THs74YGpE-JRy8ggR9uDV9lL_mTcwhfB" target="_blank">Signal_PPG_Subj_27</a></td>
</tr>
<tr>
    <td>Sujeto 28</td>
    <td>45</td>
    <td>Femenino</td>
    <td>NO</td>
    <td>120</td>
    <td>78</td>
    <td>70</td>
    <td>NO</td>
    <td>Normotenso</td>
    <td>Prehipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1Q2zvGcrKzv3l4hlt5r5pg-fC12rKr5yf" target="_blank">Signal_PPG_Subj_28</a></td>
</tr>
<tr>
    <td>Sujeto 29</td>
    <td>50</td>
    <td>Femenino</td>
    <td>SI</td>
    <td>135</td>
    <td>83</td>
    <td>76</td>
    <td>SI</td>
    <td>Prehipertenso</td>
    <td>Hipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1XqZfRx-XUJ92g3ZzPIofhn02wZx-KfHi" target="_blank">Signal_PPG_Subj_29</a></td>
</tr>
<tr>
    <td>Sujeto 30</td>
    <td>45</td>
    <td>Masculino</td>
    <td>NO</td>
    <td>111</td>
    <td>78</td>
    <td>72</td>
    <td>NO</td>
    <td>Normotenso</td>
    <td>Normotenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1mlqlQn9Y8l-khZ1vDmBk1CtX7qo9v4g6" target="_blank">Signal_PPG_Subj_30</a></td>
</tr>
<tr>
    <td>Sujeto 31</td>
    <td>46</td>
    <td>Masculino</td>
    <td>SI</td>
    <td>129</td>
    <td>82</td>
    <td>72</td>
    <td>SI</td>
    <td>Prehipertenso</td>
    <td>Hipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1Id-3cRP5oGDx06_9zwnKt1gcjWlWeLvg" target="_blank">Signal_PPG_Subj_31</a></td>
</tr>
<tr>
    <td>Sujeto 32</td>
    <td>50</td>
    <td>Masculino</td>
    <td>NO</td>
    <td>129</td>
    <td>79</td>
    <td>68</td>
    <td>NO</td>
    <td>Prehipertenso</td>
    <td>Prehipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1--fqem50XlJWkxlEy1M8dd_mMEbZbw2N" target="_blank">Signal_PPG_Subj_32</a></td>
</tr>
<tr>
    <td>Sujeto 33</td>
    <td>64</td>
    <td>Masculino</td>
    <td>NO</td>
    <td>125</td>
    <td>75</td>
    <td>78</td>
    <td>NO</td>
    <td>Prehipertenso</td>
    <td>Prehipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1UHYmYqSy5Vs7JwdhVW-k_wg3Oo1HrPj_" target="_blank">Signal_PPG_Subj_33</a></td>
</tr>
<tr>
    <td>Sujeto 34</td>
    <td>48</td>
    <td>Masculino</td>
    <td>NO</td>
    <td>130</td>
    <td>87</td>
    <td>80</td>
    <td>NO</td>
    <td>Prehipertenso</td>
    <td>Hipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1eJ9S_UgdSGQwSfAt05pA76d5L2-ycR-f" target="_blank">Signal_PPG_Subj_34</a></td>
</tr>
<tr>
    <td>Sujeto 35</td>
    <td>62</td>
    <td>Masculino</td>
    <td>SI</td>
    <td>153</td>
    <td>88</td>
    <td>84</td>
    <td>SI</td>
    <td>Hipertenso</td>
    <td>Hipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1B9JryfI-_cZN10IiB5qsi5A7grwxvVpb" target="_blank">Signal_PPG_Subj_35</a></td>
</tr>
<tr>
    <td>Sujeto 36</td>
    <td>55</td>
    <td>Masculino</td>
    <td>NO</td>
    <td>122</td>
    <td>72</td>
    <td>81</td>
    <td>NO</td>
    <td>Prehipertenso</td>
    <td>Prehipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1tJ7-zACzI3PwiF5psoQ-f3PEyblsKscG" target="_blank">Signal_PPG_Subj_36</a></td>
</tr>
<tr>
    <td>Sujeto 37</td>
    <td>57</td>
    <td>Masculino</td>
    <td>NO</td>
    <td>127</td>
    <td>80</td>
    <td>83</td>
    <td>NO</td>
    <td>Prehipertenso</td>
    <td>Hipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1o1u-kNcHyE6EfvNeaGJxh3VvzX-RwQ70" target="_blank">Signal_PPG_Subj_37</a></td>
</tr>
<tr>
    <td>Sujeto 38</td>
    <td>63</td>
    <td>Masculino</td>
    <td>NO</td>
    <td>121</td>
    <td>87</td>
    <td>68</td>
    <td>NO</td>
    <td>Prehipertenso</td>
    <td>Hipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1GQkD8Kc6m3V4ZVKuNNb4mfrxY8q0vdLv" target="_blank">Signal_PPG_Subj_38</a></td>
</tr>
<tr>
    <td>Sujeto 39</td>
    <td>48</td>
    <td>Masculino</td>
    <td>NO</td>
    <td>132</td>
    <td>83</td>
    <td>90</td>
    <td>NO</td>
    <td>Prehipertenso</td>
    <td>Hipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1cxB-Crs2PwiIbzgbyTTjo17WUieQ5BCw" target="_blank">Signal_PPG_Subj_39</a></td>
</tr>
<tr>
    <td>Sujeto 40</td>
    <td>65</td>
    <td>Femenino</td>
    <td>NO</td>
    <td>116</td>
    <td>79</td>
    <td>106</td>
    <td>NO</td>
    <td>Normotenso</td>
    <td>Normotenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1wT59vzC7vGc3CrsfYFfX5xHp36nO_zSs" target="_blank">Signal_PPG_Subj_40</a></td>
</tr>

<tr>
    <td>Sujeto 41</td>
    <td>60</td>
    <td>Masculino</td>
    <td>SI</td>
    <td>140</td>
    <td>91</td>
    <td>54</td>
    <td>SI</td>
    <td>Hipertenso</td>
    <td>Hipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1iUDVX7flGcK1RgC51g11n8-FZsLk0FYj" target="_blank">Signal_PPG_Subj_41</a></td>
</tr>
<tr>
    <td>Sujeto 42</td>
    <td>60</td>
    <td>Femenino</td>
    <td>SI</td>
    <td>144</td>
    <td>86</td>
    <td>68</td>
    <td>SI</td>
    <td>Hipertenso</td>
    <td>Hipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1UoLrM7lnHd79ZqjfdD-k6J3AjTKTR2uU" target="_blank">Signal_PPG_Subj_42</a></td>
</tr>
<tr>
    <td>Sujeto 43</td>
    <td>45</td>
    <td>Femenino</td>
    <td>NO</td>
    <td>154</td>
    <td>96</td>
    <td>65</td>
    <td>NO</td>
    <td>Hipertenso</td>
    <td>Hipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1NdkzHuZUeUeYxBG9scuYf3-k3i2DTTKx" target="_blank">Signal_PPG_Subj_43</a></td>
</tr>
<tr>
    <td>Sujeto 44</td>
    <td>53</td>
    <td>Femenino</td>
    <td>SI</td>
    <td>164</td>
    <td>93</td>
    <td>62</td>
    <td>NO</td>
    <td>Hipertenso</td>
    <td>Hipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1SS2HKH1eQkVr8_ZUC9ZcI8-PHdsZwktB" target="_blank">Signal_PPG_Subj_44</a></td>
</tr>
<tr>
    <td>Sujeto 45</td>
    <td>45</td>
    <td>Femenino</td>
    <td>SI</td>
    <td>142</td>
    <td>90</td>
    <td>69</td>
    <td>SI</td>
    <td>Hipertenso</td>
    <td>Hipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1IiBLVf2avjILcqFvdAR2-9_OltVQO4kQ" target="_blank">Signal_PPG_Subj_45</a></td>
</tr>
<tr>
    <td>Sujeto 46</td>
    <td>56</td>
    <td>Femenino</td>
    <td>NO</td>
    <td>145</td>
    <td>90</td>
    <td>69</td>
    <td>NO</td>
    <td>Hipertenso</td>
    <td>Hipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1h8_6tmBXuRtjXXU9z_2U9ojbIbSId1US" target="_blank">Signal_PPG_Subj_46</a></td>
</tr>
<tr>
    <td>Sujeto 47</td>
    <td>46</td>
    <td>Femenino</td>
    <td>SI</td>
    <td>118</td>
    <td>75</td>
    <td>86</td>
    <td>SI</td>
    <td>Normotenso</td>
    <td>Normotenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1nnkqHXF30kQYCb1s-qQ0GZ0OGpKmDokp" target="_blank">Signal_PPG_Subj_47</a></td>
</tr>
<tr>
    <td>Sujeto 48</td>
    <td>45</td>
    <td>Femenino</td>
    <td>NO</td>
    <td>107</td>
    <td>68</td>
    <td>97</td>
    <td>NO</td>
    <td>Normotenso</td>
    <td>Normotenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1BQQDKtCnhGiO9QhI9XuqCYXoGGGYqEvG" target="_blank">Signal_PPG_Subj_48</a></td>
</tr>
<tr>
    <td>Sujeto 49</td>
    <td>45</td>
    <td>Femenino</td>
    <td>NO</td>
    <td>118</td>
    <td>62</td>
    <td>72</td>
    <td>NO</td>
    <td>Normotenso</td>
    <td>Normotenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1iDB3zgPEdP-voJ5e8FcZvL-JW9ISQoxP" target="_blank">Signal_PPG_Subj_49</a></td>
</tr>
<tr>
    <td>Sujeto 50</td>
    <td>55</td>
    <td>Masculino</td>
    <td>NO</td>
    <td>119</td>
    <td>74</td>
    <td>81</td>
    <td>NO</td>
    <td>Normotenso</td>
    <td>Normotenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1PNwYOmsYQy5yUQQMX8F5-8h9rT5HLFqO" target="_blank">Signal_PPG_Subj_50</a></td>
</tr>
<tr>
    <td>Sujeto 51</td>
    <td>57</td>
    <td>Masculino</td>
    <td>NO</td>
    <td>114</td>
    <td>75</td>
    <td>83</td>
    <td>NO</td>
    <td>Normotenso</td>
    <td>Normotenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1g8pG-d5w7gDVNIfBO48WtQmSkhBsJN6g" target="_blank">Signal_PPG_Subj_51</a></td>
</tr>
<tr>
    <td>Sujeto 52</td>
    <td>58</td>
    <td>Femenino</td>
    <td>SI</td>
    <td>128</td>
    <td>72</td>
    <td>75</td>
    <td>SI</td>
    <td>Prehipertenso</td>
    <td>Prehipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1mY0T9p47wZdLjbOH0WtnD38m98vzSmwW" target="_blank">Signal_PPG_Subj_52</a></td>
</tr>
<tr>
    <td>Sujeto 53</td>
    <td>65</td>
    <td>Masculino</td>
    <td>SI</td>
    <td>121</td>
    <td>75</td>
    <td>75</td>
    <td>NO</td>
    <td>Prehipertenso</td>
    <td>Prehipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1VjmjFSG6cCJ3BseZUdNHEcIQjwhF9-NP" target="_blank">Signal_PPG_Subj_53</a></td>
</tr>
<tr>
    <td>Sujeto 54</td>
    <td>58</td>
    <td>Masculino</td>
    <td>SI</td>
    <td>134</td>
    <td>85</td>
    <td>76</td>
    <td>NO</td>
    <td>Prehipertenso</td>
    <td>Hipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1P95wSZvkqIar2rV1sSYG3yNdp7R3eNzJ" target="_blank">Signal_PPG_Subj_54</a></td>
</tr>
<tr>
    <td>Sujeto 55</td>
    <td>45</td>
    <td>Masculino</td>
    <td>SI</td>
    <td>128</td>
    <td>83</td>
    <td>71</td>
    <td>SI</td>
    <td>Prehipertenso</td>
    <td>Hipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1o1bgl6rShiGKX7Y8Hks0Lh7pIGQgDum1" target="_blank">Signal_PPG_Subj_55</a></td>
</tr>
<tr>
    <td>Sujeto 56</td>
    <td>46</td>
    <td>Femenino</td>
    <td>SI</td>
    <td>128</td>
    <td>89</td>
    <td>78</td>
    <td>SI</td>
    <td>Prehipertenso</td>
    <td>Hipertenso</td>
    <td><a href="https://drive.google.com/uc?export=download&id=1X-Q5S2sfIgkkrLu6w5HgPWXxj-bNRo7e" target="_blank">Signal_PPG_Subj_56</a></td>
</tr>

    </tbody>

<button id="clearFiltersButton">Borrar filtros</button>

</table>



<script>
    var originalData = [];

    document.querySelectorAll('#data tbody tr').forEach(function(row) {
        originalData.push({
            sujeto: row.cells[0].textContent,
            age: parseInt(row.cells[1].textContent),
            genero: row.cells[2].textContent,
            diagnostico: row.cells[3].textContent,
            systolicBP: parseInt(row.cells[4].textContent),
            diastolicBP: parseInt(row.cells[5].textContent),
            heartRate: parseInt(row.cells[6].textContent),
            tratamiento: row.cells[7].textContent,
            jnc: row.cells[8].textContent,
            aha: row.cells[9].textContent,
            archivos: row.cells[10].querySelector('a').getAttribute('href'),
            archivosText: row.cells[10].textContent
        });
    });

    document.getElementById('ageFilter').addEventListener('change', filterTable);
    document.getElementById('genderFilter').addEventListener('change', filterTable);
    document.getElementById('jncFilter').addEventListener('change', filterTable);
    document.getElementById('ahaFilter').addEventListener('change', filterTable);
    document.getElementById('clearFiltersButton').addEventListener('click', clearAllFilters);

    function filterTable() {
        var ageFilter = document.getElementById('ageFilter').value;
        var genderFilter = document.getElementById('genderFilter').value;
        var jncFilter = document.getElementById('jncFilter').value;
        var ahaFilter = document.getElementById('ahaFilter').value;

        var filteredData = originalData.filter(function(row) {
            var ageCondition = true;
            var genderCondition = true;
            var jncCondition = true;
            var ahaCondition = true;

            if (ageFilter === 'below40') {
                ageCondition = row.age < 40;
            } else if (ageFilter === 'between40and50') {
                ageCondition = row.age >= 40 && row.age <= 50;
             } else if (ageFilter === 'between51and60') {
                ageCondition = row.age >= 51 && row.age <= 60;
            } else if (ageFilter === 'above60') {
                ageCondition = row.age > 60;
            }

            if (genderFilter !== 'all') {
                genderCondition = row.genero === genderFilter;
            }

            if (jncFilter !== 'all') {
                jncCondition = row.jnc === jncFilter;
            }

            if (ahaFilter !== 'all') {
                ahaCondition = row.aha === ahaFilter;
            }

            return ageCondition && genderCondition && jncCondition && ahaCondition;
        });

        var tbody = document.querySelector('#data tbody');
        tbody.innerHTML = '';

        filteredData.forEach(function(row) {
            var newRow = document.createElement('tr');
            newRow.innerHTML = `
                <td>${row.sujeto}</td>
                <td>${row.age}</td>
                <td>${row.genero}</td>
                <td>${row.diagnostico}</td>
                <td>${row.systolicBP}</td>
                <td>${row.diastolicBP}</td>
                <td>${row.heartRate}</td>
                <td>${row.tratamiento}</td>
                <td>${row.jnc}</td>
                <td>${row.aha}</td>
                <td><a href="${row.archivos}" target="_blank">${row.archivosText}</a></td>
            `;
            tbody.appendChild(newRow);
        });
    }

    function clearAllFilters() {
        document.getElementById('ageFilter').value = 'all';
        document.getElementById('genderFilter').value = 'all';
        document.getElementById('jncFilter').value = 'all';
        document.getElementById('ahaFilter').value = 'all';

        filterTable();
    }
</script>




    </tbody>
</table>





<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Descargar archivo ZIP desde Google Drive</title>
</head>
<body>

<h2>Descargar archivo ZIP</h2>
<p>Puedes descargar el archivo ZIP que conttiene todas las señales haciendo clic en el siguiente enlace:</p>
<a href="https://drive.google.com/uc?export=download&id=1UVQOvVOoh8rKtGqEAFNf3vvDE0JTOz1x" target="_blank">Descargar archivo ZIP</a>














