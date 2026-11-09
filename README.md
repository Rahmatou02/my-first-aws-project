## Introducing Today's Project!

### Project overview

In this project, I will demonstrate how to Amazon S 3 to store and retrieve any amount of data. I'm doing this project to learn how to create, store and resolve errors in my S3 file.

### Tools and concepts

Services I used were AWS. Key concepts I learnt include create an S3 bucket in AWS, upload files and objects to my bucket, configure a static website, make object in my website visible to the public, and also added a bucket policy to my bucket.

### Time, challenges, and wins

This project took me approximately less than 20 minutes The most challenging part was make the object in the bucket public.I had to use a littel help .It was most rewarding to challenge to do actually finally getting to see the objects and files from my bucket run live and pulic was the most rewarding pat of it all.

### ❤️ Thanks for doing this project!

I chose to do this project today because i so much whant to know how things are been save and hosted on the cloud. Something that would make learning with NextWork even better is so far i have no complaints honestly. I enjoyed the lesson.

## How I Set Up an S3 Bucket

### What I did in this step

In this step, I will create and open an AWS  S3 bucket because i need space to store my websites files

### How long it took to create the bucket

Creating an S3 bucket took me less than 5 minutes.

### Region selection

The Region I picked for my S3 bucket was Europe (Frankfurt) because it is the regin closest to me.

### Understanding bucket name uniqueness

S3 bucket names are globally unique! This means no one can use the name you used on less you delete it.

![How I Set Up an S3 Bucket](https://nextwork.ai/nostalgic_cyan_innocent_alligator/uploads/70e2d059-31ab-5f67-8c58-f5edbd451140_ba6d42ad)

## Upload Website Files to S3

### What I did in this step

In this step, I will downlad an HTML file that ets up my wesite, download a zip file of images because there is no files in my bucket my bucket is still empty I needfiles in y bucket in other to host it.

### Files I uploaded

I uploaded two files to my S3 bucket - they were an index HTML file (this determines the structure i.e what goes inside) and a folder of images and asets i.e this will fill in the website with images and things to look at.

### How the files work together

Both files are necessary for this project as index.HTML determines the structure but the sturcture alone does not ilustrste the content of the website i.e the index.HTML says insert image here, it might not have the iage to display  you might have to supply that file separately. That's why have multiple files uploaded the index.HTML file to direct what's inside the websiye page but also a bunch of assets like images that the website is trying to dispay

![Upload Website Files to S3](https://nextwork.ai/nostalgic_cyan_innocent_alligator/uploads/70e2d059-31ab-5f67-8c58-f5edbd451140_a265af88)

## Static Website Hosting on S3

### What I did in this step

In this step, I will make my website available to the world this is called static website hosting and it's important because our website files will stay as just files and not turn into websites if i skip this step

### Understanding website hosting

Website hosting means putting our website files on a webserver which is a computer that can turn our files into a webpage that people can visit.

### How I enabled website hosting

To enable website hosting with my S3 bucket, I went into the porperties tab of my bucket and enabled the static web hosting and labeld index.html as my index document

### Access Control Lists (ACLs)

An ACL is an Access control list is a way to configure permission settings inside a bucket. We enable ACLs so that we can control access to our website files later. ACLs there was a pop-up mentioning that AWS recommends disablling ACLs but we will keep that enabled to learn how ACLs work and compare it with bucket policies later.

![Static Website Hosting on S3](https://nextwork.ai/nostalgic_cyan_innocent_alligator/uploads/70e2d059-31ab-5f67-8c58-f5edbd451140_c22c54c0)

## Bucket Endpoints

### Understanding bucket endpoint URLs

Once static website is enabled, S3 produces a bucket endpoint URL, which is a URL that takes you takes you to the website that you are hosting.

### What I saw when I tested the endpoint

When I first visited the bucket endpoint URL, I saw  an error and that error is called the 403 forbidden error.The reason for this error was that object in this bucket are public by defualt. Even though i have switched off block all public access the website files themselves are still completely private. I need to manage thier access ssttings privately. They need to be made public too so the public can  see the content of my website.

![Bucket Endpoints](https://nextwork.ai/nostalgic_cyan_innocent_alligator/uploads/70e2d059-31ab-5f67-8c58-f5edbd451140_22ce4daf)

## Success!

### What I did in this step

In this step, I will make the website files in my S3 bucket publicy accessible because this will enable us to view the content of my website.

### How I resolved the 403 error

To resolve this 403 Forbidden error, I scrolled all the way to the top and selected the object tab, selected the index.html file and the folder website assets. And then in th action dropdown I choose the make public using acl to solve the error.

### ✅ What were the key services and concepts you learnt in this project?

Services I used were AWS Key concepts I learnt include how to create an S3 buckets, how to use ACLs, how to upload files onto the web, configure a static website.

### ✅ How long did it take you to complete this project?

This project took me approximately less than 20 minutes to complete. The most challenging part was the bucket enpoints URL where it show error after i have make it public, It was most rewarding to do after the error was rectified.

### ❤️ Thanks for doing this project!

I chose to do this project today because i am curious of whatgoes on behind the scenes of all the websites we see and get to use on a daily bases.Something that would make learning with NextWork even better is i will like nextwork to improve on the answer tabs because sometimes you'd answer a queston and it will take you back.

![Success!](https://nextwork.ai/nostalgic_cyan_innocent_alligator/uploads/70e2d059-31ab-5f67-8c58-f5edbd451140_5d4474f9)

## Bucket Policies

### What I did in this extension

In this project extension I'm about to use bucket policies to control access to oour bucket files.  I'm doing this so that I can  stop people from deleting my file

### Understanding bucket policies

An alternative to ACLs are bucket policies, which are rules that determine whois allowed or not allowed to do something.The benefit of using bucket policies is you can have greater controls of the access of the actions or people aren't allowed to do. while ACLs are useful for controling public access to individual

![Bucket Policies](https://nextwork.ai/nostalgic_cyan_innocent_alligator/uploads/70e2d059-31ab-5f67-8c58-f5edbd451140_sm2sm2sm)

### What my bucket policy does

My bucket policy prevents the files in my bucket from being deleted. I tested this by delete a file in m S3 bucket and saw failed to delete objects.
