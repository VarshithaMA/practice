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
