3rd program (jenkins)
github : create new repo(test) copy the link 
vs code :write simple java(myfile.java) code put it inside github repo file c:....../test
          git bash: cd "path"
          git clone " http:/....../test"
          cd test
          git add myfile.java
          git commit -m "done"
          git push
jenkins:new item :test
        choose frestyle ->ok
        souce code manager :git 
                            change to main
                            choose hook(optional)
                            build steps (execute windows... code(javac myfile.java)
                            save
        build now : correct marks
______________________________________________________________________________________________
4TH 
package exp1.exp1;

import java.io.FileReader;

import org.json.simple.JSONObject;
import org.json.simple.parser.JSONParser;

public class example2 {

    public static void main(String[] args) throws Exception {

        JSONParser jsonparser = new JSONParser();

        FileReader filereader = new FileReader(".\\jsonfile\\exp.json");

        Object obj = jsonparser.parse(filereader);

        JSONObject empobj = (JSONObject) obj;

        String fname = (String) empobj.get("fname");
        String lname = (String) empobj.get("lname");

        System.out.println(fname);
        System.out.println(lname);
    }
}

___________________________________
<dependency>
    <groupId>com.googlecode.json-simple</groupId>
    <artifactId>json-simple</artifactId>
    <version>1.1</version>
    <scope>compile</scope>
</dependency>
________________________
{
	"fname":"varshitha",
	"lname":"Nayak"
}_______________
