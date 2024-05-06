# Comparing `tmp/tsforecasting-1.2.76-py3-none-any.whl.zip` & `tmp/tsforecasting-1.2.80-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,17 @@
-Zip file size: 16329 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat      391 b- defN 23-Nov-12 12:08 tsforecasting/__init__.py
--rw-rw-rw-  2.0 fat     3314 b- defN 23-Nov-19 01:20 tsforecasting/evaluation.py
--rw-rw-rw-  2.0 fat     7032 b- defN 23-Nov-19 18:53 tsforecasting/forecasting.py
--rw-rw-rw-  2.0 fat     1685 b- defN 23-Nov-20 22:15 tsforecasting/parameters.py
--rw-rw-rw-  2.0 fat    12591 b- defN 23-Nov-19 18:05 tsforecasting/treatment.py
--rw-rw-rw-  2.0 fat    13651 b- defN 23-Nov-19 18:53 tsforecasting/variational.py
--rw-rw-rw-  2.0 fat     1078 b- defN 23-Nov-27 22:14 tsforecasting-1.2.76.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     9479 b- defN 23-Nov-27 22:14 tsforecasting-1.2.76.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Nov-27 22:14 tsforecasting-1.2.76.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-Nov-27 22:14 tsforecasting-1.2.76.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      925 b- defN 23-Nov-27 22:14 tsforecasting-1.2.76.dist-info/RECORD
-11 files, 50252 bytes uncompressed, 14761 bytes compressed:  70.6%
+Zip file size: 21050 bytes, number of entries: 15
+-rw-rw-rw-  2.0 fat        0 b- defN 24-May-06 20:48 configs/__init__.py
+-rw-rw-rw-  2.0 fat     2776 b- defN 24-May-06 20:48 configs/parameters.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-May-06 20:48 models/__init__.py
+-rw-rw-rw-  2.0 fat    27183 b- defN 24-May-06 20:48 models/forecasting_models.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-May-06 20:48 performance/__init__.py
+-rw-rw-rw-  2.0 fat     5852 b- defN 24-May-06 20:48 performance/evaluation.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-May-06 20:48 processing/__init__.py
+-rw-rw-rw-  2.0 fat    11777 b- defN 24-May-06 20:48 processing/processor.py
+-rw-rw-rw-  2.0 fat        0 b- defN 24-May-06 20:48 training/__init__.py
+-rw-rw-rw-  2.0 fat    11206 b- defN 24-May-06 21:34 training/validation.py
+-rw-rw-rw-  2.0 fat     1078 b- defN 24-May-06 21:49 tsforecasting-1.2.80.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     9731 b- defN 24-May-06 21:49 tsforecasting-1.2.80.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-06 21:49 tsforecasting-1.2.80.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       61 b- defN 24-May-06 21:49 tsforecasting-1.2.80.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1200 b- defN 24-May-06 21:49 tsforecasting-1.2.80.dist-info/RECORD
+15 files, 70956 bytes uncompressed, 19058 bytes compressed:  73.1%
```

## zipnote {}

```diff
@@ -1,34 +1,46 @@
-Filename: tsforecasting/__init__.py
+Filename: configs/__init__.py
 Comment: 
 
-Filename: tsforecasting/evaluation.py
+Filename: configs/parameters.py
 Comment: 
 
-Filename: tsforecasting/forecasting.py
+Filename: models/__init__.py
 Comment: 
 
-Filename: tsforecasting/parameters.py
+Filename: models/forecasting_models.py
 Comment: 
 
-Filename: tsforecasting/treatment.py
+Filename: performance/__init__.py
 Comment: 
 
-Filename: tsforecasting/variational.py
+Filename: performance/evaluation.py
 Comment: 
 
-Filename: tsforecasting-1.2.76.dist-info/LICENSE
+Filename: processing/__init__.py
 Comment: 
 
-Filename: tsforecasting-1.2.76.dist-info/METADATA
+Filename: processing/processor.py
 Comment: 
 
-Filename: tsforecasting-1.2.76.dist-info/WHEEL
+Filename: training/__init__.py
 Comment: 
 
-Filename: tsforecasting-1.2.76.dist-info/top_level.txt
+Filename: training/validation.py
 Comment: 
 
-Filename: tsforecasting-1.2.76.dist-info/RECORD
+Filename: tsforecasting-1.2.80.dist-info/LICENSE
+Comment: 
+
+Filename: tsforecasting-1.2.80.dist-info/METADATA
+Comment: 
+
+Filename: tsforecasting-1.2.80.dist-info/WHEEL
+Comment: 
+
+Filename: tsforecasting-1.2.80.dist-info/top_level.txt
+Comment: 
+
+Filename: tsforecasting-1.2.80.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `tsforecasting/treatment.py` & `processing/processor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,299 +1,261 @@
+import numpy as np
 import pandas as pd
 import datetime
 from dateutil.relativedelta import relativedelta
 from sklearn.ensemble import (
-    RandomForestRegressor,
-    ExtraTreesRegressor,
-    GradientBoostingRegressor
-    )
+        RandomForestRegressor,
+        ExtraTreesRegressor,
+        GradientBoostingRegressor
+        )
 
 
-class Treatment:
+class Processing:
     def __init__(self):
         self.target = 'y'
-
-    def round_cols(self,
-                   dataset: pd.DataFrame,
-                   round_: int = 5):
-    
-        X=dataset.copy()
-        
-        num_cols=[col for col in X.select_dtypes(include=['float', 'float64','float32']).columns if col != self.target]
-        for col in num_cols: X[[col]]=X[[col]].round(round_)
-            
-        return X
+        self.date_cols = []
+        self.input_cols = []
+        self.target_cols = []
     
     def slice_timestamp(self, 
-                        dataset: pd.DataFrame):
+                        dataset:pd.DataFrame):
         """
-        Extracts timestamp column 'Date' and moves target column to the end of the DataFrame.
-        Converts timestamp column into specific format ('%Y-%m-%d %H:%M:%S').
+        Detects all columns in the DataFrame that are date or datetime related, including those with timezones.
+    
         Args:
             dataset (pd.DataFrame): Input DataFrame.
+        """
+        
+        X = dataset.copy()
+
+        # Loop through columns and detect different types of datetime data
+        for col in X.columns:
+            if pd.api.types.is_datetime64_any_dtype(X[col]):
+                self.date_cols.append(col)
+                            
+        for col in self.date_cols:
+            # Format the datetime column
+            X[col] = pd.to_datetime(X[col].dt.strftime('%Y-%m-%d %H:%M:%S'))
         
+        if 'Date' in self.date_cols:
+            X.index = X['Date']
+                
+        return X  
+    
+    def engin_date(self, 
+                   dataset: pd.DataFrame,
+                   drop: bool = True):
+        """
+        Engineer date-related features from datetime columns in the input DataFrame.
+    
+        Args:
+            dataset (pd.DataFrame): Input DataFrame.
+            drop (bool, optional): Whether to drop original datetime columns after feature creation. Defaults to True.
+    
         Returns:
-            pd.DataFrame: DataFrame with datetime timestamp formatted and target column moved to the end.
+            pd.DataFrame: DataFrame with newly engineered date-related features.
         """
-        X=dataset.copy()
-        X=X[[col for col in X.columns if col != self.target] + [self.target]]
+
+        # Identify columns that are datetime
+        X = self.slice_timestamp(dataset).copy()
         
-        for col in list(X.columns):
-            if col=='Date': X['Date']=pd.to_datetime(X['Date'].dt.strftime('%Y-%m-%d %H:%M:%S'))
+        # Dataframe to store new features
+        X_ = pd.DataFrame(index=X.index)
+
+        # Loop through each datetime column to create date-related features directly
+        for col in list(set(self.date_cols)):
+
+            X_[col + '_day_of_month'] = X[col].dt.day
+            X_[col + '_day_of_week'] = X[col].dt.dayofweek + 1
+            X_[col + '_is_weekend'] = (X[col].dt.dayofweek >= 5).astype(int)
+            X_[col + '_month'] = X[col].dt.month
+            X_[col + '_day_of_year'] = X[col].dt.dayofyear
+            X_[col + '_year'] = X[col].dt.year
+            X_[col + '_hour'] = X[col].dt.hour
+            X_[col + '_minute'] = X[col].dt.minute
+            X_[col + '_second'] = X[col].dt.second
+            # Optionally drop the original datetime column
+            if drop:
+                X = X.drop(col, axis=1)
+                
+        # Concatenate the new features at the beginning of the DataFrame
+        X = pd.concat([X_, X], axis=1)
+    
         return X
     
-
-    def multivariable_lag(self,
-                          dataset: pd.DataFrame,
-                          range_lags: list = [1,10],
-                          drop_na: bool = True):
+    def make_timeseries(self, 
+                        dataset: pd.DataFrame,
+                        window_size: int, 
+                        horizon: int, 
+                        granularity : str = '1d',
+                        datetime_engineering : bool = True):
         """
-        Creates lag features for the target "y" variable within a specified range of lags.
+        Transforms a DataFrame into a single DataFrame containing sequential windows and horizon predictions,
+        including NaNs where full horizon data isn't available. This allows using all available data for training up to the last point.
 
         Args:
-            dataset (pd.DataFrame): Input DataFrame.
-            range_lags (list, optional): Range of lag intervals. Defaults to [1, 10].
-            drop_na (bool, optional): Whether to drop rows with NA values. Defaults to True.
-
+            dataset (pd.DataFrame): A DataFrame with at least a 'y' column for time series data and a 'Date' column.
+            window_size (int): The number of time steps in each window, indicating how many past observations each input sample includes.
+            horizon (int): The number of time steps to predict into the future, which sets how far ahead the labels are relative to the end of each window.
+            granularity (str): granularity of datetime column: 1m,30m,1h,1d,1wk,1mo (default='1d')
         Returns:
-            pd.DataFrame: DataFrame with lag features added.
+            pd.DataFrame: A DataFrame where each row represents a window of observations and horizon predictions,
+                          starting with the date of the window, followed by lag features, and then horizon predictions.
+
+        Raises:
+            ValueError: If the `window_size` is larger than the input array length, which would make windowing impossible.
         """
-        assert range_lags[0]>=1, 'Range lags first interval value should be bigger then 1'
-        assert range_lags[0]<=range_lags[1], 'Range lags first interval value should be bigger then second'
         
-        X=dataset.copy()
-        X_=X.copy()
-        X_=self.slice_timestamp(X_)
-    
-        for e in range(range_lags[0],range_lags[1]+1):
-            lag_str=str(e)
-            lag_str=self.target+'_lag_'+lag_str
-            df=pd.DataFrame({'target':X[self.target],
-                          lag_str:X[self.target].shift(e)
-                          })
-            df=df.drop('target',axis=1)
-            X_[lag_str]=df[lag_str]
-        cols,input_cols=list(X_.columns),list(X_.columns)
-        input_cols.remove(self.target)
-        last_col=cols[len(cols)-1:]
-        if drop_na==True:
-            X_=X_.dropna(axis=0, subset=last_col)
-        elif drop_na==False:
-            X_[input_cols]=X_[input_cols].apply(lambda x: x.fillna(x.mean()),axis=0)
-        for col in cols:
-            if col=='Date':
-                X_=X_.set_index(['Date']) 
-                break
+        if window_size > len(dataset):
+            raise ValueError("The lags length (window_size) cannot exceed the length of the time_series.")
+
+        time_series = dataset[self.target].values
+        date_series = dataset['Date'].values  
+
+        # Calculate the maximum index for creating windows
+        max_window_index = len(time_series) - window_size
+
+        # Create windows and corresponding dates
+        windows = np.array([time_series[i:i + window_size] for i in range(max_window_index + 1)])
             
-        return X_
+        extended_dates = np.array([date_series[window_size:][-1] + pd.Timedelta(granularity, n=i + 1) for i in range(1)])
+        date_col = np.concatenate([date_series[window_size:], extended_dates])
+        date_col = pd.to_datetime(date_col, unit='ns')
+        
+        # Create horizons, allowing NaNs for the future windows
+        horizons = np.array([time_series[i + window_size:i + window_size + horizon] if i + window_size + horizon <= len(time_series)
+                             else np.concatenate([time_series[i + window_size:len(time_series)], np.full((i + window_size + horizon - len(time_series)), np.nan)])
+                             for i in range(max_window_index + 1)])
+
+        # Column names for windows and horizons
+        self.lag_cols = [f'y_lag_{i+1}' for i in range(window_size)]
+        self.horizon_cols = [f'y_horizon_{i+1}' for i in range(horizon)]
+
+        # Create DataFrame for lags and horizons
+        lag_df = pd.DataFrame(windows, columns=self.lag_cols)
+        horizon_df = pd.DataFrame(horizons, columns=self.horizon_cols)
+
+        # Combine into one DataFrame
+        X = pd.concat([lag_df, horizon_df], axis=1).reset_index(drop=True)
+        X.insert(0, 'Date', date_col)
+        
+        if datetime_engineering:
+            X = self.engin_date(dataset = X,
+                                drop = True)
+        
+        self.target_cols = [col for col in X.columns if 'horizon' in col]
+        self.input_cols = [col for col in X.columns if col not in self.target_cols]
+        
+        return X
     
-    def future_timestamps(self,
-                          dataset: pd.DataFrame,
-                          forecast_size: int,
-                          granularity: str ='1d'):
+    def future_timestamps(self, dataset: pd.DataFrame, horizon: int, granularity: str = '1d'):
         """
         Generates future timestamps based on the last timestamp in the input dataset.
-        
+    
         Args:
             dataset (pd.DataFrame): Input DataFrame with a 'Date' column.
-            forecast_size (int): Number of future timestamps to generate.
+            horizon (int): Number of future timestamps to generate.
             granularity (str, optional): Granularity of timestamps ('1m', '30m', '1h', '1d', '1wk', '1mo'). Defaults to '1d'.
-        
+    
         Returns:
             pd.DataFrame: DataFrame with generated future timestamps.
         """
-        X=dataset.copy()
-        X=self.slice_timestamp(X)
-
-        timestamp,timestamp_list=list((X.Date[len(X)-1:]))[0],[]
-        
-        if granularity=='1m':
-        
-            def generate_datetimes(date_from_str=timestamp, days=1000):
-               date_from=datetime.datetime.strptime(str(date_from_str), '%Y-%m-%d %H:%M:%S')
-               for n in range(1,1420*days):
-                   yield date_from + datetime.timedelta(minutes=n)
-            for date in generate_datetimes():
-                timestamp_list.append((date.strftime('%Y-%m-%d %H:%M:%S')))
-                
-        elif granularity=='30m':
-        
-            def generate_datetimes(date_from_str=timestamp, days=1000):
-               date_from=datetime.datetime.strptime(str(date_from_str), '%Y-%m-%d %H:%M:%S')
-               for n in range(1,1420*days):
-                   yield date_from + datetime.timedelta(minutes=30*n)
-            for date in generate_datetimes():
-                timestamp_list.append((date.strftime('%Y-%m-%d %H:%M:%S')))
-        
-        elif granularity=='1h':
-        
-            def generate_datetimes(date_from_str=timestamp, days=1000):
-               date_from=datetime.datetime.strptime(str(date_from_str), '%Y-%m-%d %H:%M:%S')
-               for hour in range(1,24*days):
-                   yield date_from + datetime.timedelta(hours=hour)
-            for date in generate_datetimes():
-                timestamp_list.append((date.strftime('%Y-%m-%d %H:%M:%S')))
-            
-        elif granularity=='1d':
         
-            def generate_datetimes(date_from_str=timestamp, days=1000):
-               date_from=datetime.datetime.strptime(str(date_from_str), '%Y-%m-%d %H:%M:%S')
-               for day in range(1,days):
-                   yield date_from + datetime.timedelta(days=day)
-            for date in generate_datetimes():
-                timestamp_list.append((date.strftime('%Y-%m-%d %H:%M:%S')))
-
-        elif granularity=='1wk':
-                
-            def generate_datetimes(date_from_str=timestamp, weeks=1000):
-               date_from=datetime.datetime.strptime(str(date_from_str), '%Y-%m-%d %H:%M:%S')
-               for week in range(1,weeks):
-                   yield date_from + datetime.timedelta(weeks=week)
-            for date in generate_datetimes():
-                timestamp_list.append((date.strftime('%Y-%m-%d %H:%M:%S')))
-        
-        elif granularity=='1mo':
-        
-            def generate_datetimes(date_from_str=timestamp, months=100):
-               date_from=datetime.datetime.strptime(str(date_from_str), '%Y-%m-%d %H:%M:%S')
-               for month in range(0,months):
-                   yield date_from + relativedelta(months=month+1)
-            for date in generate_datetimes():
-                timestamp_list.append((date.strftime('%Y-%m-%d %H:%M:%S')))
-        
-        X_=pd.DataFrame()
-        X_['Date']=timestamp_list
-        X_['Date']=pd.to_datetime(X_['Date'])
-        
-        X_=X_.iloc[0:forecast_size,:]
+        X = self.slice_timestamp(dataset).copy()
         
-        return X_
-
-    @staticmethod
-    def engin_date(dataset: pd.DataFrame,
-                   drop: bool = True):
-        """
-        Engineer date-related features in the input DataFrame.
-
-        Args:
-            dataset (pd.DataFrame): Input DataFrame.
-            drop (bool, optional): Whether to drop original datetime columns. Defaults to True.
-
-        Returns:
-            pd.DataFrame: DataFrame with engineered date-related features.
-        """
-        # This method is responsible for engineering date-related features in the input DataFrame X.
-        # It can also optionally drop the original datetime columns based on the 'drop' parameter.
-        X=dataset.copy()
-        # Extract the data types of each column in X and create a DataFrame x.
-        x=pd.DataFrame(X.dtypes)
-        # Create a 'column' column to store the column names.
-        x['column']=x.index
-        # Reset the index and drop the original index column.
-        x=x.reset_index().drop(['index'], axis=1).rename(columns={0:'dtype'})
-        # Filter for columns with datetime data type.
-        a=x.loc[x['dtype'] == 'datetime64[ns]']
-    
-        # Initialize an empty list to store the names of datetime columns.
-        date_columns=[]
-    
-        # Loop through datetime columns.
-        for date_col in a['column']:
-            date_columns.append(date_col)
-            # Convert datetime values to a standardized format (Year-Month-Day Hour:Minute:Second).
-            X[date_col]=pd.to_datetime(X[date_col].dt.strftime('%Y-%m-%d %H:%M:%S'))
-    
-        # Define a function to create additional date-related features for a given column.
-        def create_date_features(X, col):
-            # Extract day of the month, day of the week, and whether it's a weekend.
-            X[col + '_day_of_month']=X[col].dt.day
-            X[col + '_day_of_week']=X[col].dt.dayofweek + 1
-            X[[col + '_is_wknd']]=X[[col + '_day_of_week']].replace([1, 2, 3, 4, 5, 6, 7],
-                                                                                  [0, 0, 0, 0, 0, 1, 1])
-            X[col + '_month']=X[col].dt.month
-            X[col + '_day_of_year']=X[col].dt.dayofyear
-            X[col + '_year']=X[col].dt.year
-            X[col + '_hour']=X[col].dt.hour
-            X[col + '_minute']=X[col].dt.minute
-            X[col + '_second']=X[col].dt.second
-    
-            return X
-    
-        # Loop through the list of date columns and create the additional features using the defined function.
-        for col in date_columns:
-            X=create_date_features(X, col)
-            # If 'drop' is set to True, drop the original datetime column.
-            if drop == True: X=X.drop(col, axis=1)
+        last_date = pd.to_datetime(X['Date'].iloc[-1])
+        timestamp_list = []
     
-        # Return the DataFrame X with the engineered date-related features.
-        return X
+        if granularity == '1m':
+            delta = datetime.timedelta(minutes=1)
+        elif granularity == '30m':
+            delta = datetime.timedelta(minutes=30)
+        elif granularity == '1h':
+            delta = datetime.timedelta(hours=1)
+        elif granularity == '1d':
+            delta = datetime.timedelta(days=1)
+        elif granularity == '1wk':
+            delta = datetime.timedelta(weeks=1)
+        elif granularity == '1mo':
+            delta = relativedelta(months=1)
+        else:
+            raise ValueError("Unsupported granularity provided.")
+    
+        for _ in range(horizon):
+            last_date += delta
+            timestamp_list.append(last_date)
     
+        return pd.DataFrame({'Date': timestamp_list})
 
     @staticmethod
-    def feature_selection_tb(dataset: pd.DataFrame,
-                             target: str = 'y',
-                             relevance: float = 0.99,
-                             algo: str = 'ExtraTrees',
-                             estimators: int = 250):
+    def treebased_feature_selection(dataset: pd.DataFrame,
+                                    target: str = 'y',
+                                    relevance: float = 0.99,
+                                    algo: str = 'ExtraTrees',
+                                    estimators: int = 250):
         """
-        Perform feature selection using tree-based algorithms (RandomForest,ExtraTrees,GBR).
-
-        Args:
-            dataset (pd.DataFrame): Input DataFrame.
-            target (str, optional): Target variable column name. Defaults to 'y'.
-            relevance (float, optional): Total feature importance to retain. Defaults to 0.99.
-            algo (str, optional): Tree-based algorithm ('ExtraTrees', 'RandomForest', 'GBR'). Defaults to 'ExtraTrees'.
-            estimators (int, optional): Number of estimators for the algorithm. Defaults to 250.
-
+        Conducts feature selection based on the importance derived from specified tree-based regression models.
+        This method aims to retain a subset of features whose cumulative importance meets a predefined threshold, thus facilitating model interpretability and efficiency.
+    
+        Parameters:
+            dataset (pd.DataFrame): The dataset containing both features and the target variable.
+            target (str, optional): The name of the target variable column. Defaults to 'y'.
+            relevance (float, optional): The cumulative feature importance threshold to retain. Valid values range from 0.5 to 1.0. Defaults to 0.99.
+            algo (str, optional): Specifies the tree-based regression algorithm to use for assessing feature importance. 
+                                  Options include 'ExtraTrees', 'RandomForest', and 'GBR' (Gradient Boosting Regressor). Defaults to 'ExtraTrees'.
+            estimators (int, optional): The number of trees to build in the model. More trees can increase the accuracy but also the computational cost. Defaults to 250.
+    
         Returns:
-            tuple: Selected columns and DataFrame with feature importances.
+            tuple:
+                - list: The names of the selected columns that meet the relevance threshold.
+                - pd.DataFrame: A DataFrame with two columns: 'variable' and 'percentage', indicating the feature names and their respective importances.
+    
+        Raises:
+            AssertionError: If 'relevance' is not between 0.5 and 1.0.
         """
-        assert relevance>=0.5 and relevance<=1 , 'relevance value should be in [0.5,1[ interval'
-        
-        train=dataset.copy()
-        train=train[[col for col in train.columns if col != target] + [target]] # target to last index
-       
-        X_train=train.iloc[:, 0:(len(list(train.columns))-1)].values
-        y_train=train.iloc[:, (len(list(train.columns))-1)].values
-        
-        if algo=='RandomForest':
-            fs_model=RandomForestRegressor(n_estimators=estimators)
-            fs_model.fit(X_train, y_train)
-        elif algo=='ExtraTrees':
-            fs_model=ExtraTreesRegressor(n_estimators=estimators)
-            fs_model.fit(X_train, y_train)
-        elif algo=='GBR':
-            fs_model=GradientBoostingRegressor(n_estimators=estimators)
-            fs_model.fit(X_train, y_train)
-    
-        column_imp=fs_model.feature_importances_
-        column_names=list(train.columns).copy()
-        column_names.remove(target)
-        
-        Columns,feat_imp=pd.Series(column_names),pd.Series(column_imp)
-        
-        X=pd.concat([feat_imp,Columns],axis=1)
-        X=X.rename(columns={0:'percentage',1:'variable'})
-        
-        n=0.015
-        va_df=X[X['percentage'] > n]
-        val=va_df['percentage'].sum()
-        for iteration in range(0,10):
-                
-            if val<=relevance:
-                va_df=X[X['percentage']>n]
-                n=n*0.5
-                val=va_df['percentage'].sum()
-            elif val>relevance:
+        # Validate the relevance input to ensure it is within the acceptable range.
+        assert 0.5 <= relevance <= 1, 'Relevance value should be within the [0.5, 1.0] interval.'
+    
+        # Preparing the data, separating features and target
+        train = dataset.copy()
+        features = [col for col in train.columns if col != target]
+        X_train = train[features].values
+        y_train = train[target].values
+        
+        # Selecting the model based on the algorithm specified
+        if algo == 'RandomForest':
+            model = RandomForestRegressor(n_estimators=estimators)
+        elif algo == 'ExtraTrees':
+            model = ExtraTreesRegressor(n_estimators=estimators)
+        elif algo == 'GBR':
+            model = GradientBoostingRegressor(n_estimators=estimators)
+        else:
+            raise ValueError(f"Unsupported algorithm '{algo}'. Choose from 'RandomForest', 'ExtraTrees', 'GBR'.")
+    
+        # Fitting the model and obtaining feature importances
+        model.fit(X_train, y_train)
+        importances = model.feature_importances_
+    
+        # Creating a DataFrame of feature importances
+        feat_imp_df = pd.DataFrame({
+            'variable': features,
+            'percentage': importances
+        }).sort_values(by='percentage', ascending=False)
+        
+        # Determining the features whose cumulative importance meets the relevance threshold
+        cumulative_importance = 0.0
+        selected_features = []
+        for _, row in feat_imp_df.iterrows():
+            selected_features.append(row['variable'])
+            cumulative_importance += row['percentage']
+            if cumulative_importance >= relevance:
                 break
-        va_df=va_df.sort_values(['percentage'], ascending=False)
     
-        sel_cols=[]
-        for rows in va_df['variable']: sel_cols.append(rows)
-        sel_cols.append(target)
-        
-        return sel_cols, va_df
+        # Return the list of selected feature names and the feature importance DataFrame
+        return selected_features, feat_imp_df
+
+
```

## Comparing `tsforecasting-1.2.76.dist-info/LICENSE` & `tsforecasting-1.2.80.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tsforecasting-1.2.76.dist-info/METADATA` & `tsforecasting-1.2.80.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsforecasting
-Version: 1.2.76
+Version: 1.2.80
 Summary: TSForecasting is an Automated Time Series Forecasting Framework
 Home-page: https://github.com/TsLu1s/TSForecasting
 Author: Luís Santos
 Author-email: luisf_ssantos@hotmail.com
 License: MIT
 Keywords: data science,machine learning,time series forecasting,automated time series,multivariate time series,univariate time series,automated machine learning,automl
 Classifier: Intended Audience :: Education
@@ -23,27 +23,28 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas (>=1.4.4)
 Requires-Dist: numpy (>=1.23.5)
 Requires-Dist: python-dateutil (>=2.8.2)
 Requires-Dist: scikit-learn (>=1.2.2)
-Requires-Dist: pmdarima (>=2.0.1)
+Requires-Dist: autogluon (>=1.1.0)
+Requires-Dist: lightgbm (>=4.3.0)
 Requires-Dist: xgboost (>=1.7.4)
-Requires-Dist: h2o (>=3.44.0.1)
-Requires-Dist: prophet (>=1.1.2)
+Requires-Dist: catboost (>=1.2.2)
+Requires-Dist: tqdm (>=4.65.2)
 
 <br>
 <p align="center">
   <h2 align="center"> TSForecasting - Automated Time Series Forecasting Framework
   <br>
   
 ## Framework Contextualization <a name = "ta"></a>
 
-The `TSForecasting` project constitutes an complete and integrated pipeline to Automate Time Series Forecasting applications through the implementation of multivariate approaches integrating regression models referring to modules such as `SKLearn`, `H2O.ai`, `XGBoost` and also univariate approaches of more classics methods such as `Prophet` and `AutoArima`, this following an 'Expanding Window' performance evaluation.
+The `TSForecasting` project offers a comprehensive and integrated pipeline designed to Automate Time Series Forecasting applications. By implementing multivariate approaches that incorporate multiple regression models, it combines multiple relevant modules such as `SKLearn`, `AutoGluon`, `CatBoost` and `XGBoost`, following an `Expanding Window` structured approach for performance evaluation ensuring a robust, scalable and optimized forecasting solution.
 
 The architecture design includes five main sections, these being: data preprocessing, feature engineering, hyperparameter optimization, forecast ensembling and forecasting method selection which are organized and customizable in a pipeline structure.
 
 This project aims at providing the following application capabilities:
 
 * General applicability on tabular datasets: The developed forecasting procedures are applicable on any data table associated with any Time Series Forecasting scopes.
 
@@ -52,18 +53,19 @@
 * Robustness and improvement of predictive results: The implementation of the TSForecasting pipeline aims to improve the predictive performance directly associated with the application of the best performing forecasting method. 
    
 #### Main Development Tools <a name = "pre1"></a>
 
 Major frameworks used to built this project: 
 
 * [Sklearn](https://scikit-learn.org/stable/)
-* [H2O.ai](https://docs.h2o.ai/h2o/latest-stable/h2o-docs/automl.html)
+* [AutoGluon](https://auto.gluon.ai/stable/index.html)
+* [CatBoost](https://catboost.ai/)
 * [XGBoost](https://xgboost.readthedocs.io/en/stable/)
-* [AutoArima](https://alkaline-ml.com/pmdarima/modules/generated/pmdarima.arima.auto_arima.html)
-* [Prophet](https://facebook.github.io/prophet/docs/quick_start.html#python-api)
+* [LightGBM](https://lightgbm.readthedocs.io/en/latest/Installation-Guide.html)
+
     
 ## Performance Evaluation Structure <a name = "ta"></a>
 
 <p align="center">
   <img src="https://i.ibb.co/ctYj6tt/Expanding-Window-TSF.png" align="center" width="450" height="350" />
 </p>  
     
@@ -90,102 +92,99 @@
 
 # Usage Examples
     
 ## 1. TSForecasting - Automated Time Series Forecasting
     
 The first needed step after importing the package is to load a dataset and define your DataTime (`datetime64[ns]` type) and Target column to be predicted, then rename them to `Date` and `y`, respectively.
 The following step is to define your future running pipeline parameters variables, these being:
-* train_size: Length of Train data in which will be applied the first Expanding Window iteration;  
-* forecast_size: Full length of test/future ahead predictions;
-* sliding_size: Length of sliding window, sliding_size>=forecast_size is suggested;
-* models: Select all the models intented to ensemble to evaluation. To fit and compare predictive performance of available models set them in paramater `models:list`, options are the following:
+* train_size: Length of Train data in which will be applied the first Expanding Window iteration;
+* lags: The number of time steps in each window, indicating how many past observations each input sample includes;
+* horizon: Full length of test/future ahead predictions;
+* sliding_size: Length of sliding window, sliding_size>=horizon is suggested;
+* models: All selected models intented to be ensembled for evaluation. To fit and compare predictive performance of available models set them in paramater `models:list`, options are the following:
   * `RandomForest`
   * `ExtraTrees`
   * `GBR`
   * `KNN`
   * `GeneralizedLR`
   * `XGBoost`
-  * `H2O_AutoML`
-  * `AutoArima`
-  * `Prophet`
+  * `LightGBM`
+  * `Catboost`
+  * `AutoGluon`
+
 * hparameters: Nested dictionary in which are contained all models and specific hyperparameters configurations. Feel free to customize each model as you see fit (customization example shown bellow); 
 * granularity: Valid interval of periods correlated to data -> 1m,30m,1h,1d,1wk,1mo (default='1d');
 * metric: Default predictive evaluation metric is `MAE` (Mean Absolute Error), other options are `MAPE` (Mean Absolute Percentage Error) and `MSE`
 (Mean Squared Error);
  
-The `fit_forecast` method set the default parameters for fitting and comparison of all segmented windows for each selected and configurated model. After implementation, the `history` method agregates the returning variables `fit_performance` containing every detailed measure of each `window` iteration predicted value and `fit_predictions` measuring all segmented `window` iterations performance.
+The `fit_forecast` method set the default parameters for fitting and comparison of all segmented windows for each selected and configurated model. After implementation, the `history` method agregates the returning the variable `fit_performance` containing the detailed measures of each window iteration forecasted value and all segmented iterations performance.
 
 The `forecast` method forecasts the future values based on the previously predefined best performing model.
         
 ```py
 
-from tsforecasting.forecasting import TSForecasting
-from tsforecasting.parameters import model_configurations
+from tsforecasting.forecasting import (TSForecasting,
+                                       model_configurations)
 import pandas as pd
 import warnings
 warnings.filterwarnings("ignore", category=Warning) #-> For a clean console
-import h2o
-
-h2o.init() # -> Run only if using H2O_AutoML models   
 
 ## Dataframe Loading
 data = pd.read_csv('csv_directory_path') 
 data = data.rename(columns={'DateTime_Column': 'Date','Target_Name_Column':'y'})
 data = data[['Date',"y"]]
     
 ## Get Models Hyperparameters Configurations
 parameters = model_configurations()
 print(parameters)
 
 # Customization Hyperparameters Example
-parameters["RandomForest"]["n_estimators"] = 200
-parameters["KNN"]["n_neighbors"] = 5
-parameters["Prophet"]["seasonality_mode"] = 'multiplicative'
-parameters["H2O_AutoML"]["max_runtime_secs"] = 90
+hparameters["RandomForest"]["n_estimators"] = 50
+hparameters["KNN"]["n_neighbors"] = 5
+hparameters["Catboost"]["iterations"] = 150
+hparameters["AutoGluon"]["time_limit"] = 50
 
 ## Fit Forecasting Evaluation
-tsf = TSForecasting(train_size = 0.95,
-                    forecast_size = 15,
-                    sliding_size = 15,
-                    models = ['RandomForest','ExtraTrees', 'GBR', 'KNN', 'GeneralizedLR',
-                              'XGBoost', 'AutoArima','Prophet','H2O_AutoML'],
-                    hparameters = parameters,
-                    granularity = "1h", # 1m,30m,1h,1d,1wk,1mo
-                    metric = "MAE"      # MAPE, MSE
+tsf = TSForecasting(train_size = 0.90,
+                    lags = 10,
+                    horizon = 10,
+                    sliding_size = 30,
+                    models = ['RandomForest', 'GeneralizedLR', 'GBR', 'KNN', 'GeneralizedLR',
+                              'XGBoost', 'LightGBM', 'Catboost', 'AutoGluon'],
+                    hparameters = hparameters,
+                    granularity = '1h',
+                    metric = 'MAE'
                     )
 tsf = tsf.fit_forecast(dataset = data)
 
 # Get Fit History
-fit_predictions, fit_performance = tsf.history()
+fit_performance = tsf.history()
 
 ## Forecast
 forecast = tsf.forecast()
 
 ```  
 
 ## 2. TSForecasting - Extra Auxiliar Methods
-    
-The `engin_date` method converts and transforms columns of Datetime type into additional columns (Year, Day of the  Year, Season, Month, Day of the month, Day of the week, Weekend, Hour, Minute, Second) which will be added by association to the input dataset and subsequently deletes the original column if parameter `drop`=`True`.
 
-The `multivariable_lag` method creats all the past lags related to the target `y` feature automatically (in accordance to `range_lags` parameter) and adds each constructed column into the dataset.
+The `make_timeseries` method transforms a DataFrame into a format ready for time series analysis. This transformation prepares data sets for forecasting future values based on historical data, optimizing the input for subsequent model training and analysis, taking into consideration both the recency of data and the horizon of the prediction.
+
+* window_size: Determinates how many past observations each sample in the DataFrame should include. This creates a basis for learning from historical data.
+* horizon: Defines the number of future time steps to forecast. This addition provides direct targets for prediction models.
+* granularity: Adjusts the temporal detail from minutes to months, making the method suitable for diverse time series datasets (options -> 1m,30m,1h,1d,1wk,1mo).
+* datetime_engineering: When activated enriches the dataset with extra date-time features, such as year, month, and day of the week, potentialy enhancing the predictive capabilities of the model.
  
 ```py   
 
-# Feature Engineering 
-
-from tsforecasting.treatment import Treatment
+from tsforecasting.forecasting import Processing
 
-tr = Treatment()
+pr = Processing()
 
-data = tr.engin_date(dataset = data,
-                     drop = False) 
+data = pr.make_timeseries(dataset=data, window_size=10, horizon=2, granularity='1h')
 
-data = tr.multivariable_lag(dataset = data,
-                            range_lags = [1,10],
-                            drop_na = True)    
 ```
     
 ## License
 
 Distributed under the MIT License. See [LICENSE](https://github.com/TsLu1s/TSForecasting/blob/main/LICENSE) for more information.
 
 ## Contact
```

