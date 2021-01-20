 # starreviews
 
A flutter package for displaying detailed star reviews

<img src=https://github.com/buraktabn/starreviews/raw/master/images/example.png width="200" />

## Install

```yaml
dependencies:  
  starreviews:
    git: https://github.com/nibaji/starreviews.git
```

```console
$  flutter pub get
```

```dart
import  'package:starreviews/starreviews.dart';
```

## Usage

```dart
List<String> _names = ['⭐⭐⭐⭐⭐', '⭐⭐⭐⭐', '⭐⭐⭐', '⭐⭐', '⭐'];  
List<double> _values = [0.5, 0.2, 0.8, 0.5, 0.1];
```
```dart
StarReviews(  
    total: 20,  
    starNames: _names,  
    values: _values,  
    showPercentage: true,  
    average: 3.2,
)
```
```dart
StarReviewsHorizontal(
    total: 30,
    starNames: _names,
    showProgressBarBorder: false,
    valueColor: Colors.black,
    progressBarBackgroundColor: Colors.grey.withOpacity(0.4),
    values: _values,
    showPercentage: true,
    starColor: Colors.black,
    average: 4.2,
)
```

## Customization
Here is a list of properties available to customize the widget:

|        Name        	|       Type      	|                 Description                	|
|:------------------:	|:---------------:	|:------------------------------------------:	|
| total| int| total numbers of reviews           	|
| showHeader| bool| if false, hides header           	|
| showBottom| bool| if false, hides bottom reviews           	|
| showPercentage| bool| if false, hides rating number           	|
| starNames| List<String>| list of star names (max 5)           	|
| percentageStyle| TextStyle| style applied to percentage                                  	|
| showPercentage| bool| if false, hides percentage                                 	|
| valueColor| Color| color of the progressbar             	|
| progressBarBackgroundColor| Color| color of the progress bar background                      	|
| values| List<double>| list of review values as `double`                     	|
| starSize| double| the size of the stars                     	|
| starColor| Color| the color of the stars                     	|
| average| double| the average number that'll be displayed                     	|
| showProgressBarBorder| bool| option to hide borders of the progress bar                     	|
| lineHeight| double| height of the progress bar                     	|
| spaceBetween| double| the space between progress bars                     	|

  
## Contributions

Contributions of any kind are more than welcome! Feel free to fork and improve in any way you want, make a pull request, or open an issue.
