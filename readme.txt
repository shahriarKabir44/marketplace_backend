GET requests:
/getnotiff/:id ->get notifications of the user id=:id

/showcusts/:pd -> get customers of the product pd

/find/:cid/:pid -> find whether :cid is a customer of :pid

/logout -> logout user
/userStat -> current user
/posts/:id -> get ads posted by user id=:id

/myCart/:id -> cart of user :id

/showProduct/:id -> product page of :id

/products/ -> all products

/relate/:pid/:cid -> find relationship between product pid and customer cid

/users -> number of users 

/showUs/:id -> get propic and fullname of user :id

POST requests:

/signup -> register user. requires: pwd, fname, lname, uname, email, propic, imagname, phone
/login -> loging user. requires: uname, pwd

/sendnotif -> send notification. requires: from, pd, to, type, barg, order, notifType
/addtocart -> add a product to cart.  requires: to,pd,from,barg, time,status
/update/:id -> update user id=:id. requires: fname, lname, mail, pwd, phn

/postAd ->post an ad . requires: img1, img2, img3, img4, askedPrc, postedBy, date, type, details, img1name, img2name, img3name, img4name

/setpropic -> set propic of an user. requires: ID, propic, imagname

/removeCt ->remove a product from cart. requires: prID, cusID, ownerID
/removnotif -> remove a notification . requires:  sender, reciever, prod, type 
