# openENTRANCE: Model linkage mappings and definitions

Copyright 2020 openENTRANCE consortium

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

     http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.

## Model linkage mappings and definitions

<p align="center">
  <img width="195" height="195" src="https://github.com/openENTRANCE/model-linkage/blob/master/assets/Models.png">
</p>

This repository aims to share the mapping of some models to be used in [openENTRANCE](https://openentrance.eu/) is based on these three principles:

* Define the hierarchical relations among the different concepts used for variable and region domains of the **common data format**
* Define a set of consistent names, definitions, and meanings for the different concepts

The first rule is to define a single set of pre-defined reserved words to be used in the data-exchange platform. A reserved word can’t be used for two different concepts in the platform.
The **common data format** are thought to be valid both for dynamic data, changing over time (e.g., hourly data), and static data (e.g., yearly data). Besides, we will need to represent both deterministic data (those for which there is certainty over the evolution of the corresponding data) and stochastic data, which depend on uncertain scenarios.
Within the **common data format**, there are six dimensions:

1.	Model
2.	Scenario
3.	Region
4.	Variable
5.	Unit
6.	Subannual

Next, we describe in detail the information to be provided in each dimension. This definition must be exhaustive (cover all the data in the models considered) and avoid duplicities that might lead to inconsistencies. That is, all data should be defined once and just once.

## 1. Model
This dictionary of model can be linked through this exchange format. Given the intended openness of the exchange format, models inside and outside the openENTRANCE consortium are welcome. A brief description of the model is provided in the next link. Model name and version will be specified as follows:

> openTEPES|1.6.12

The model suite:

|  __Model__  |  __Version__  |
|-------------|---------------|
| EMPIRE      |               |
| e-Transport |               |
| EXIOMOD     | 2.0.0        |
| FanSi       |               |
| FRESH:COM   |               |
| GENeSYS-MOD |               |
| HERO        |               |
| openTEPES   | 1.6.12        |
| OSCARS      |               |
| Plan4EU     |               |
| REMES-EU    |               |
| SCOPE-SD    |               |

More details could be found [here](Model/ModelDictionary.md).

## 2. Scenario
The analysis/case scenario name describes the type of analysis to be carried out and its context, as used in the openENTRANCE project. For example, scenario **GreenGrowth** or **Distributed PV all over Europe** or **Centralized utility-scale PV in southern Europe** can be possible names of scenarios. ***Any name is valid here***.
This field can be extended to refer to the fact that the scenario considered is stochastic/random to account, for example, for the spatial correlation of wind/solar generation, or demand, in different regions/countries. Stochastic/random data are usually time dependent.
Thus, stochastic/random scenario names can be used. For example, possible names can be:

> Distributed PV all over Europe|Scen001 

Where the data given belong to the random scenario **Scen001** of the analysis scenario **Distributed PV all over Europe**.

<!-- <table>
<tr><th>Table 1 Heading 1 </th><th>Table 1 Heading 2</th></tr>
<tr><td>

|Table 1| Middle | Table 2|
|--|--|--|
|a| not b|and c |

</td><td>

|b|1|2|3|
|--|--|--|--|
|a|s|d|f|

</td></tr> </table> -->
