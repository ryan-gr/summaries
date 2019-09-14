# Bash

Bash reminds me of the days when I was younger - when a multitidue of things seemed so much simpler, while others seemed so impossible to grasp that I couldn't wait to move on with life.  

When I realized that variables couldn't be 'set' if there were spaces between the equals sign and values (i.e. `variable = value`), I thought it was weird. Oh how was I naive.

`if` and `for` loops were interesting as well,

```if [ "$variable" == "value" ]; then  
  echo Wow! Something is happening!  
fi```

```
for item in ${array[@]}; do  
  echo $item  
done
```

I mean look at that $ynt@x! fi? array[@]? wow.  

However, there was a certain beauty in the simplicity of the language. It was nice being able to concatenate variables and strings without using an operator.  

`echo $var1 $var2 is actually not $var3 $var4`

Liberating!  

But looping through a file.. just what.

```
list=()  
while IFS= read -d $'\0' -r line ; do  
  file_list=("${list[@]}" "$line")  
done < <(find . -print0)  
```
> based on https://stackoverflow.com/questions/8213328/store-the-output-of-find-command-in-an-array/8213509

I was reminded on how I thought batch's way of looping through a file line by line was bad.. but now I'm thankful for batch.

Batch is an interesting language to code in. Infinitely useful for people that live on the command line, but you can tell that its been around the block for awhile.
