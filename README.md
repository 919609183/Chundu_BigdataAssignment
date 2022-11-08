https://beam.apache.org/get-started/quickstart-java/

mvn archetype:generate `
  -D archetypeGroupId=org.apache.beam `
  -D archetypeArtifactId=beam-sdks-java-maven-archetypes-examples `
  -D archetypeVersion=2.42.0 `
  -D groupId=org.example `
  -D artifactId=word-count-beam `
  -D version="0.1" `
  -D package=org.apache.beam.examples `
  -D interactiveMode=false
   
cd .\word-count-beam

dir .\src\main\java\org\apache\beam\examples

In the word-count-beam directory, create a file called sample.txt. Add some text to the file. For this example

mvn compile exec:java -D exec.mainClass=org.apache.beam.examples.WordCount `
 -D exec.args="--inputFile=sample.txt --output=counts" -P direct-runner

ls counts*
   
more counts*

Output :

power: 1
before: 1
still: 1
should: 3
quick: 1
like: 2
wax: 1
sinners: 1
wilt: 1
tend: 1
virtue: 1
joy: 1
Madness: 1
assay: 1
own: 1
further: 1
sugar: 1
come: 1
death: 2
consummation: 1
blown: 1
pause: 1
grief: 2
honey: 1
Prince: 1
right: 1
tell: 1
thank: 1
enough: 2
returns: 1
tune: 1
your: 13
Grating: 1
pangs: 1
here: 3
at: 1
set: 1
patient: 1
would: 3
A: 1
helps: 1
poor: 1
confusion: 1
contumely: 1
er: 4
offences: 1
OPHELIA: 15
sometime: 1
The: 15
-- More  --

