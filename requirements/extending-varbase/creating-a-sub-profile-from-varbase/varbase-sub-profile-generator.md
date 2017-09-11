# Varbase Sub Profile Generator

We do have a generator for new Varbase sub profiles, which could help you in a quick way.

## Step #1
Download the Varbase Sub profile generator from https://bitbucket.org/Vardot/varbase-subprofile-generator and get ready to generate profiles.

**For Example:** if /var/www/html/products is your products working directory you could do the following

```
mkdir /var/www/html/products
cd /var/www/html/products
git clone git@bitbucket.org:Vardot/varbase-subprofile-generator.git
cd /var/www/html/products/varbase-subprofile-generator
```

## Step #2
Set the version of the generator

**For Example:** if you want to generate a sub profile to use Varbase 8.4.08 you could do the following:

```
cd /var/www/html/products/varbase-subprofile-generator
git checkout 8.4.08
```

## Step #3
Run the generate command:

**For Example:** If we want to create a new Varbase sub profile named **cv** , we could run the following commands in your local terminal:

```
cd /var/www/html/products/varbase-subprofile-generator
bash create-new-varbase-subprofile.sh "cv" -vvv
```
After that you will have a new **cv** sub p**rofile cv-project** as you can see in the following:

```
cd /var/www/html/products/varbase-subprofile-generator
ll
create-new-varbase-subprofile.sh
cv/
cv-project/
.git/
README.md
settings.yml
varbase_subprofile_basic/
varbase-subprofile-basic-project/
```

## Step #4
Copy your Varbase sub profile to your working directory.

**For Example:** You could copy **cv** and **cv-project** to your local products development working directory:
```
mv /var/www/html/products/varbase-subprofile-generator/cv /var/www/html/products/cv
mv /var/www/html/products/varbase-subprofile-generator/cv-project /var/www/html/products/cv-project

```

## Step #5
You will need to create 2 new **PRIVATE** repositories for your sub profile

 **For Example:**  


https://bitbucket.org/Vardot/cv
https://bitbucket.org/Vardot/cv-project

Then we could add the remote repositories

```


```



