### Stylesheet

This document is a set of code conventions to be used at EuVou project. 

* 1. [[Naming|Stylesheet#1-nomeação]]
* 2. [[Formatting|Stylesheet#2-formatação]]
* 3. [[Comments|Stylesheet#3-comentários]]
* 4. [[Good Practices|Stylesheet#4-boas-práticas]]

***

#### 1. Nomeação

**1.1.** Usar camelCase para nomear atributos.

``` Java

    //exemplo bom
    private bool isUserLoggedIn;

    //exemplo ruim
    private bool isuserloggedin;

```

**1.2.** Usar camelCase para nomear métodos and parâmetros.

``` Java

    //exemplo bom
    private void setCurrentUserId(int currentUserId){
        this.currentUserId = currentUserId;
    }

    //exemplo ruim
    private void setcurrentuserid(int currentuserid){
        this.currentUserId = currentUserId;
    }
```

**1.3.** TO nome do método deve representar o que ele faz, usando um verbo.

``` Java

    //exemplo bom
    private void registerUser(User user){
        UserDAO userDAO = new UserDAO(getActivity());

        userDAO.saveUser(user);
    }

    //exemplo ruim
    private void userRegistration(User user){
        UserDAO userDAO = new UserDAO(getActivity());

        userDAO.saveUser(user);
    }

```

**1.4.** Usar PascalCase para nomear classes e interfaces.

``` Java

    //exemplo bom
    public class EventException extends Exception{
        public EventException(String message){
            super(message);
        }
    }

    //exemplo ruim
    public class eventexception extends Exception{
        public EventException(String message){
            super(message);
        }
    }
```

**1.5.** Usar nomes significativos para nomear atributos. Abreviações não devem ser usadas.

``` Java

    //exemplo bom
    private EditText birthDateField;

    //exemplo ruim
    private EditText bdField;

```

**1.6.**  Não devem haver nomes de atributos com apenas um caractere, como `a`, `b`, `c`. Exceto para o caractere `i` em loops. 

``` Java

    //exemplo bom
    private View top5RankView;

    //exemplo ruim
    private View v;

```

**1.7.** Constantes devem ser escritas SCREAMING_SNAKE_CASE.

``` Java

    //exemplo bom
    private int USER_STATUS;

    //exemplo ruim
    private int USERSTATUS;

```

**1.8.** Tratar acrônimos como palavras.

``` Java

    //exemplo bom
    private String urlQuery;

    //exemplo ruim
    private String URLQuery;

```

**[[Back to top|Stylesheet#stylesheet]]**

#### 2. Formatação

**2.1.** Usar TAB para indentar, com tamanho 4.

``` Java
    
    //exemplo bom
    public Integer getEvaluation(){
        return evaluation;
    }

    //exemplo ruim
    public Integer getEvaluation(){
    return evaluation;
    }

```

**2.2.** Usar uma linha em branco para separar grupos lógicos.

``` Java

    //exemplo bom
    @Override
    public boolean onCreateOptionsMenu(Menu menu){
        getMenuInflater().inflate(R.menu.menu_event_consultation, menu);
        actionBar = getSupportActionBar();

        setSearchBar(menu);
        configActionBar();

        radioGroup = (RadioGroup) findViewById(R.id.search_radio_group);
        radioGroup.setOnCheckedChangeListener(this);
        return true;
    }

    //exemplo ruim
    @Override
    public boolean onCreateOptionsMenu(Menu menu){
        getMenuInflater().inflate(R.menu.menu_event_consultation, menu);
        actionBar = getSupportActionBar();
        setSearchBar(menu);
        configActionBar();
        radioGroup = (RadioGroup) findViewById(R.id.search_radio_group);
        radioGroup.setOnCheckedChangeListener(this);
        return true;
    }

```

**2.3.** Linhas devem possuir no máximo 100 caracteres.

``` Java

    //exemplo bom
    if(userEvaluationInDataBase == null){
            query = "INSERT INTO evaluate_user(grade, idUser, idUserEvaluated) VALUES (" +
                    "\"" + evaluation.getUserRating() + "\"," +
                    "\"" + evaluation.getIdUserLoggedIn() + "\"," +
                    "\"" + evaluation.getIdUserEvaluated() + "\")";
        }  

    //exemplo ruim
    if(userEvaluationInDataBase == null){
            query = "INSERT INTO evaluate_user(grade, idUser, idUserEvaluated) VALUES (" \"" + evaluation.getUserRating() + "\","\"" + evaluation.getIdUserLoggedIn() + "\"," ,"\"" evaluation.getIdUserEvaluated() + "\")";

```

**2.4.** A chave de abertura de um método, loop ou estrutura condicional, deve estar na mesma linha, e a chave de fechamento deve estar um nível atrás do código.

``` Java

    //exemplo bom
    public Vector<String> getCategory(){
        return category;
    }

    //exemplo ruim
    public Vector<String> getCategory()
    {
        return category;
    }

```

**2.5.** Não deve haver espaços entre operadores, comparadores, `=`, `:` e `?`.

``` Java
    
    //exemplo bom
    private void setIdOwner(int idOwner){
        this.idOwner = idOwner;
    }

    //exemplo ruim
    private void setIdOwner(int idOwner){
        this.idOwner=idOwner;
    }

```

**2.6.** Não deve haver espaços depois de `(`, `[` e antes de `)`, `]`.

``` Java

    //exemplo bom
    private void setPrice(Integer price){
        this.price=price;
    }

    //exemplo ruim
    private void setPrice  ( Integer price ) {
        this.price = price;
    }

``` 

**2.7.** Em loops, deve haver espaço depois do ponto e vírgula.

``` Java

    //exemplo bom
    for(int i = 0; i < placesDataSize; i++){

               ...

                Place aux = new Place(idPlace,placeName, placeEvaluate, placeLongitude,
                        placeLatitude, placeOperationTime, placeDescription, placeAddress,
                        placePhone);

                int placesArrayListSize = places.size();

                places.add(aux);

                assert places.size() == placesArrayListSize + 1;
                assert places.get(placesArrayListSize) == aux;
     }

    //exemplo ruim
    for(int i=0;i<placesDataSize;i++){

               ...

                Place aux = new Place(idPlace,placeName, placeEvaluate, placeLongitude,
                        placeLatitude, placeOperationTime, placeDescription, placeAddress,
                        placePhone);

                int placesArrayListSize = places.size();

                places.add(aux);

                assert places.size() == placesArrayListSize + 1;
                assert places.get(placesArrayListSize) == aux;
    }

```
**2.8.** Não deve haver espaços depois do nome do método e depois de `for`, `if`, `else if` e `switch`.

``` Java

    //exemplo bom
    private boolean getUserLoginStatus(){
       boolean isUserLoggedIn = false;
       LoginUtility loginUtility = new LoginUtility(this.getActivity());

       if(loginUtility.hasUserLoggedIn()){
            isUserLoggedIn = true;
        }
        else{
            isUserLoggedIn = false;
        }
        
        return isUserLoggedIn;
    }

    //exemplo ruim
    private boolean getUserLoginStatus () {
       boolean isUserLoggedIn = false;
       LoginUtility loginUtility = new LoginUtility(this.getActivity());

       if(loginUtility.hasUserLoggedIn()) {
            isUserLoggedIn = true;
        }
        else {
            isUserLoggedIn = false;
        }
        
        return isUserLoggedIn;
    }

```


**[[Back to top|Stylesheet#stylesheet]]**

#### 3. Comentários

**3.1.** Os comentários devem ter a mesma indentação do código.

``` Java
    
    //exemplo bom
    //Sets the required adapter to adapt items of the places array in items of the places list
    PlaceAdapter placeAdapter = new PlaceAdapter(getActivity(),places);

    //exemplo ruim
    //Sets the required adapter to adapt items of the places array in items of the places list
        PlaceAdapter placeAdapter = new PlaceAdapter(getActivity(),places);

```

**3.2.** Os comentários devem começar com letra maiúscula.

``` Java
    
    //exemplo bom
    //Saves the user evaluation set at database
    UserEvaluationDAO userEvaluationDAO = new UserEvaluationDAO(getActivity());

    //exemplo ruim
    //saves the user evaluation set at database
    UserEvaluationDAO userEvaluationDAO = new UserEvaluationDAO(getActivity());

```

**3.3.** Os comentários devem ser escritos na mesma linguagem do código.

**3.4.** Deve ser usado `//` para comentários de uma linha e `/*` ... `*/` para comentários com mais de uma linha.

``` Java
    
    //exemplo bom
    /**
    * File: ShowTop5Ranking.java
    * Purpose: Show the five places with better evaluation
    */

    //exemplo ruim
    //File: ShowTop5Ranking.java
    //Purpose: Show the five places with better evaluation
```

**3.5.** Deve ser colocado @Override antes de todos métodos sobrescritos.

``` Java
    
    //exemplo bom
    @Override
    public void onCreate(Bundle savedInstanceState){
        super.onCreate(savedInstanceState);
    }

    //exemplo ruim
    public void onCreate(Bundle savedInstanceState){
        super.onCreate(savedInstanceState);
    }
```

**[[Back to top|Stylesheet#stylesheet]]**


#### 4. Boas Práticas

**4.1.** Use constantes ao invés de números e strings mágicas.

``` Java
    
    //exemplo bom
    private final Double INVALID_LATITUDE = Double.valueOf(91);
    private Double latitude = INVALID_LATITUDE;

    //exemplo ruim
    private Double latitude = Double.valueOf(91);
```

**4.2.** Um método deve realizar apenas uma tarefa.

``` Java
    
    //exemplo bom
    public JSONObject searchUserEvaluation(int userEvaluatedtId, int userId){

        final String QUERY = "SELECT * FROM evaluate_user WHERE idUser = \"" + userId
                + "\" AND idUserEvaluated = " + userEvaluatedtId;

        JSONObject userEvaluation = executeConsult(QUERY);

        return userEvaluation;
    }
```