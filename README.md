Hello! Here you can see an example of the code that I wrote for my thesis paper "Comparing the Methods of Machine Learning for Video Game Price Forecasting" (I apologize for the in-code comments made in Russian only). This code:

1) parses data from the dataset with Steam games, their prices and characteristics (steam_games_cleaned.csv);
2) limits the research range to paid indie games ($4.99-$29.99);
3) processes quantitative data about developers and publishers (the number of previously released games, the number of reviews and copies sold for previous games, their rating, etc.), using only information about games PRIOR to a specific game in the dataset to avoid future leaks;
4) processes tags (short descriptions of the distinctive features of the game) using TF-IDF;
5) Based on these features, predicts game prices using gradient boosting (LightGBM library), using TimeSeriesSplit to avoid future leaks.;
6) calculates the key metrics regarding the model's prediction quality (MAE, MSE, MedAE, MAPE, Bias, etc.);
7) displays the accuracy of predictions for different price categories ($4.99-$9.99, $10-$14.99 and so on);
8) provides information on the model's most serious errors.
   
To view or use the code:

- download both files ("Example_Code_Game_Price_Prediction.ipynb" and "steam_games_cleaned.csv");
- put these files in the same folder;
- open the file with the code "Example_Code_Game_Price_Prediction.ipynb" and click "Run All".

Добрый день! Здесь вы можете видеть пример кода, который я написал для моего диплома "Прогнозирование цен на видеоигры методами машинного обучения".
Этот код:
  1) парсит данные из датасета с играми Steam, их ценами и характеристиками (steam_games_cleaned.csv);
  2) ограничивает диапазон исследования платными инди-играми ($4.99-$29.99);
  3) обрабатывает количественные данные о разработчиках и издателях (количество ранее выпущенных игр, количество отзывов и проданных копий для предыдущих игр, их рейтинг и т. д.), используя только информацию об играх ДО конкретной игры в датасете, чтобы избежать "утечки будущего";
  4) обрабатывает тэги (краткие описания отличительных особенностей игры) с помощью TF-IDF;
  5) на основе этих признаков прогнозирует цены на игры с помощью градиентного бустинга (библиотека LightGBM), используя TimeSeriesSplit для избежания утечки будущего;
  6) выводит статистику по результатам предсказаний и их качеству (MAE, MSE, MedAE, MAPE, Bias и т. д.);
  7) анализирует точность предсказаний для разных ценовых категорий ($4.99-$9.99, $10-$14.99 и т. д.);
  8) выводит статистику по наиболее серьёзным ошибкам модели.

Чтобы проверить код:
  1) загрузите оба файла ("Example_Code_Game_Price_Prediction.ipynb" и "steam_games_cleaned.csv");
  2) поместите эти файлы в одну папку;
  3) откройте файл с кодом "Example_Code_Game_Price_Prediction.ipynb" и нажмите "Run All".
