# Continuous Distributions

Apply to __continuous variables__, or variables that can take on any value between two specified values

Have a probability __density__ function (PDF) instead of a probability mass function (PMF)


## Uniform Distribution

__Description: *Probability of any given value of x is completely random over the defined interval (a, b)*__

#### Probability Density Function

![uniform pdf img](https://upload.wikimedia.org/wikipedia/commons/thumb/9/96/Uniform_Distribution_PDF_SVG.svg/500px-Uniform_Distribution_PDF_SVG.svg.png)

PDF Equation: ![](https://wikimedia.org/api/rest_v1/media/math/render/svg/648692e002b720347c6c981aeec2a8cca7f4182f)  
Support: ![](https://wikimedia.org/api/rest_v1/media/math/render/svg/026357b404ee584c475579fb2302a4e9881b8cce)  
Paramters: ![](https://wikimedia.org/api/rest_v1/media/math/render/svg/adb722a971235b0ed2cf099e6b4d9dc3304936fa)  
Expected Value: ![](https://wikimedia.org/api/rest_v1/media/math/render/svg/83f8e71092f95652ba4e65a6916c144aa470f4ec)  
Variance: ![](https://wikimedia.org/api/rest_v1/media/math/render/svg/95f6f2aef440271aa37dec67fe279bb74e4398a4)  
            ^typo - should be 2 not 12


## Exponential Distribution

__Description: *Describes the time between events in a Poisson process*__

Is a particular case of the gamma distribution, and continuous analogue of the geometric distibution.

Is memoryless, meaning that same pattern of behavior will be expected regardless of previous history

Example: Equipment failure

#### Probability Density Function

![exponential pdf img](https://upload.wikimedia.org/wikipedia/commons/thumb/e/ec/Exponential_pdf.svg/650px-Exponential_pdf.svg.png)

PDF Equation: λe^−λx  
Support: x ∈ 0, infinity  
Paramters: λ > 0 rate, or inverse scale  
Expected Value: λ^−1 (= β)  
Variance: λ^−2 (= β2)  


## Normal (or Gaussian) Distribution

__Description: *Mean value most likley, then decreasing probability as distance from the mean*_

Very important because of the Central Limit Theorem (CLT)

Characteristic 'bell curve' shape 
            Larger standard deviation => shorter wider curve

'Standard normal curve' has total area beneath the curve equal to 1  

Empirical rule:
            68% of area under curve is within 1 std dev of mean  
            95% of area under curve is within 2 std dev of mean  
            99.7% of area under curve is within 3 std dev of mean  

Example: Distribution of heights in a population

#### Probability Density Function

![normal pdf img](https://upload.wikimedia.org/wikipedia/commons/thumb/7/74/Normal_Distribution_PDF.svg/700px-Normal_Distribution_PDF.svg.png)

PDF Equation: ![](https://wikimedia.org/api/rest_v1/media/math/render/svg/1a9287a082350af2fe84ea67da609e32f8591528)    
Support: ![](https://wikimedia.org/api/rest_v1/media/math/render/svg/a9c6d458566aec47a7259762034790c8981aefab)  
Paramters: mu, sigma^2  
Expected Value: ![](https://wikimedia.org/api/rest_v1/media/math/render/svg/2e0b88c13e96068427ea74158dc1ebd8ce63e8b5)   
Variance: ![](https://wikimedia.org/api/rest_v1/media/math/render/svg/c1aeca67847d56ce69da7d74761f189089819b8b)  


### Student's t Distribution

__Description: *Subcategory of normal distribution used for small samples (<30)*_

Heavier tails than normal distribution

Degrees of freedom drive shape of curve; more deg of freedom = 'sharper' curve = greater confidence  
            By sample size 30 (deg of freedom = 29), t-dist ~= normal dist  

#### Probability Density Function

![student t pdf img](https://upload.wikimedia.org/wikipedia/commons/thumb/4/41/Student_t_pdf.svg/650px-Student_t_pdf.svg.png)

PDF Equation: ![](https://wikimedia.org/api/rest_v1/media/math/render/svg/7fb35627dbb7e3dec4f14d60b0b58ea399966f46)    
Support: x ∈ (−∞; +∞)  
Paramters: v > 0 (deg of freedom)  
Expected Value: 0 for v > 1   
Variance: v / (v-2) for v > 2, infinity for 1 < v </= 2, otherwise undefined  


_all images taken from wikipedia_
