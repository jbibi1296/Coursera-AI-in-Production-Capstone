Usage notes
===============

All commands are from this directory.


1. Are there unit tests for the API?
 $ python ./unittests/ApiTests.py


2. Are there unit tests for the model?
 $ python model.py


3. Are there unit tests for the logging?
 $ python unittests/LoggerTests.py

4. Can all of the unit tests be run with a single script and do all of the unit tests pass?
 $python run-tests.py

5. Is there a mechanism to monitor performance?
 Run app first,

 $ python app.py

 Then, please run PerformanceMonitoring.ipinb on Jupyter Notebook

 Or, run the container to test that it is working after build the container written as below (Sec.11).
    ~$ docker run -p 4000:8080 peerreview
 Go to http://0.0.0.0:4000/ and you will see a basic website.


6. Was there an attempt to isolate the read/write unit tests from production models and logs?
 Please see run-tests.py, Logger.py, model.py

7. Does the API work as expected? For example, can you get predictions for a specific country as well as for all countries combined?
 

8. Does the data ingestion exists as a function or script to facilitate automation?
 $ python run-model-train.py

9. Were multiple models compared?
 RandomForest and SVM are compared. Please See model.py

10. Did the EDA investigation use visualizations?
 Please see images and model.py.

11. Is everything containerized within a working Docker image?
 Dockerfile is prepared. Please run following command to build.
 $ docker build -t peerreview .

12. Did they use a visualization to compare their model to the baseline model?
 Please see images and model.py.



