Kannst du für diese Klasse Tests schreiben?
Es soll FluentAssertions verwendet werden.

Die TestKlasse soll keine eigenen Properties haben, noch sollen statische Methoden verwendet werden.
Die TestClassen sollten immer sealed sein.
Die TestKlasse soll heisen wie der Name der zu testenden Klasse, zusätzlich noch mit dem Suffix "Tests" enden.

Es soll immer kommentare für 
// Arrange 
// Act
// Assert 
geben. Ggf. auch ein: 
// CleanUp.

Variablen für das zu testenden System soll immer "sut" benannt sein.

Wie die zu testende Merthode im Test ausgeführt soll das ergebnis immer in result gespeichert werden.

Im Assert sollte dann die result-Variable mit einer variable namens "expected" gegen geprüft werden.

Ziel ist eine Code Coverage von mehr als 80% zu erreicht wird.

Das namensschema der TestMethoden ist wie folgt: <MethodToBeTested>_<StateOfSystemUndTest>_<ExpectedResult>. Beispiel: Exists_FileDoesNotExist_ReturnsFalse

Ist das TestSetup mehr als 15 Zeilen, sollte dies in eine eigene Klasse ausgelagert werden.

- Es soll XUnit verwendet werden.
- Es sollen edge cases getestet werden
- Es kann Fact und Theory verwendet werden.
