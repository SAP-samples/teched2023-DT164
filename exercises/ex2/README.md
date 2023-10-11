# Exercise 2 - Scope and Organizational Structure Phase

In this exercise, we will learn to perform scoping and create organizational structure.

## Exercise 2.1 Define Scope(incl. CLT)

Please make sure that you don´t select more than 5 countries at once for the initial implementation.​
The amount of CLT enabled “Scenarios” is dependent on the content version.

1. Open Define Scope app.​

2. Select Germany & USA as countries.​

3. Choose More Countries/Regions and create Cook Islands as target country based on Germany as source country.​

4. For example, select Baseline Accelerator as scope bundle and search for IFRS and add the scenario.​

5. Select Cook Islands from the Countries/Regions filter and add a scenario just for Cook Islands (e.g. 2FD).​

6. Complete Define Scope activity.​


For more detailed instructions:​

[Define Scope](https://education.hana.ondemand.com/education/pub/cbc/index.html?show=project%21PR_4E5C20A1C2A9228F:uebung#TS_F1FF49E31A904BB69D0BB3B403C55C38) as interactive tutorial & [Define Scope](https://help.sap.com/docs/CENTRAL_BUSINESS_CONFIGURATION/55c9333eed324cd284f6c4e5dab8462f/36afd912a1a944e2ab1b07e3de2c1ed3.html?locale=en-US) documentation on SAP Help Portal​

[Localize Business Configuration](https://education.hana.ondemand.com/education/pub/cbc/index.html?show=project%21PR_9F2EF45E3070449B:uebung#2) (CLT) as interactive tutorial & [CLT EA](https://help.sap.com/doc/2f35b1b90ee74ee6a549d4cbd6ce99ba/2022_05.4/en-US/SAPCentralBusinessConfiguration_ConfigurationLocalizationTool_en-US.pdf) documentation on SAP Help Portal​

[CLT Limitations](https://launchpad.support.sap.com/#/notes/3107866)



## Exercise 2.2 Sub Exercise 2 Description

After completing these steps you will have...

1.	Enter this code.
```abap
DATA(lt_params) = request->get_form_fields(  ).
READ TABLE lt_params REFERENCE INTO DATA(lr_params) WITH KEY name = 'cmd'.
  IF sy-subrc = 0.
    response->set_status( i_code = 200
                     i_reason = 'Everything is fine').
    RETURN.
  ENDIF.

```

2.	Click here.
<br>![](/exercises/ex2/images/02_02_0010.png)

## Summary

You've now ...

Continue to - [Exercise 3 - Excercise 3 ](../ex3/README.md)
