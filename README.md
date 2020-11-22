# 3Drag LDM
This repository contains all the custom firmware for 3Drag 3D printer developed @ [+LAB](www.piulab.it)

[![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.4282564-blue)](https://doi.org/10.5281/zenodo.4282564)
![](https://img.shields.io/badge/Marlin-v1.0.3dev-orange)
![](https://img.shields.io/github/license/piuLAB-official/3Drag_LDM?color=green)
![GitHub release (latest by date)](https://img.shields.io/github/v/release/piuLAB-official/3Drag_LDM)
![](https://travis-ci.org/piuLAB-official/3Drag_LDM.svg?branch=main)

This is a custom version of the [Marlin Firmware](https://github.com/MarlinFirmware/Marlin) specifically modified for 3Drag 3D printer used in LDM mode. 

```LDM (liquid Deposition Modeling) is a particular 3D printer process in which viscous fluid are extruded from a reservoir and deposited on the build plate. This process is more generally called Direct Ink Writing (DIW).```

The firmware have been modified starting from that available from [ElettronicaIn](https://3dprint.elettronicain.it/wp-content/uploads/2016/02/Marlin_LCD_Alfa_2EXT175.zip).
_Use this firmware in combination with [3Drag LDM extruder](https://github.com/am-craft/3Drag_LDM_extruder)_

## Major modifications
- E0 thermistor and bed thermistor have been set to dummy (no heating required to extrude viscous fluids)
- _DEFAULT_AXIS_STEPS_PER_UNIT_ for E motor have been modified following this equation: ![](https://latex.codecogs.com/svg.latex?Esteps/mm=\frac{motorSteps*microsteps*gearMultiply}{8})



## About Marlin

Marlin is an optimized firmware for [RepRap 3D printers](http://reprap.org/) based on the [Arduino](https://www.arduino.cc/) platform. 
Updated Marlin firmware are available at the [Marlin Releases page](https://github.com/MarlinFirmware/Marlin/releases). Additional documentation can be found at the [Marlin Home Page](http://marlinfw.org/).


## Disclaimer

```Flashing a custom firmware happens at your own risk. THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS” AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.```
