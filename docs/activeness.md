## Group 成员动态

对组织项目内的任务，分享，日程，文件的创建，更新，评论操作记 1 分，按周复位。

查看者必须与目标用户在同一个组织，仅能查看组织可见项目和已参与的项目，并且不能看到未参与的仅参与者可见对象

### 读取成员动态 [GET /organizations/{_organizationId}/activeness/{_userId}/weekly{?startDate,limit}]

+ Parameters
    + _organizationId (ObjectID, required) - 组织 id
    + _userId (ObjectID, required) - 用户 id
    + startDate (date, required) - 本周开始时间
    + limit (number, optional) - 返回数量，最多 5 个

+ Response 200

        [{
          "_id": "5847d23cf197c9132831cb17",
          "_boundToObjectId": "5847d23cd1cb0cb3bd334c37",
          "_organizationId": "5847d23ad1cb0cb3bd334bc2",
          "_projectId": "5847d23bd1cb0cb3bd334bce",
          "_userId": "5109f1e918e6fcfc560001a6",
          "boundToObjectType": "post",
          "startDate": "2016-12-04T16:00:00.000Z",
          "updated": "2016-12-07T09:11:24.722Z",
          "created": "2016-12-07T09:11:24.722Z",
          "point": 1,
          "boundToObject": {
            "_id": "5847d23cd1cb0cb3bd334c37",
            "_creatorId": "5109f1e918e6fcfc560001a6",
            "_projectId": "5847d23bd1cb0cb3bd334bce",
            "postMode": "html",
            "source": "teambition",
            "tagIds": [],
            "visible": "members",
            "isArchived": null,
            "pin": false,
            "involveMembers": ["5109f1e918e6fcfc560001a6"],
            "updated": "2016-12-07T09:11:24.614Z",
            "created": "2016-12-07T09:11:24.614Z",
            "isDeleted": false,
            "attachments": [],
            "content": "content0",
            "title": "content0",
            "isShimoDoc": false,
            "url": "http://localhost/project/5847d23bd1cb0cb3bd334bce/posts/post/5847d23cd1cb0cb3bd334c37"
          }
        }, {
          "_id": "5847d23cf197c9132831cb18",
          "_boundToObjectId": "5847d23cd1cb0cb3bd334c3e",
          "_organizationId": "5847d23ad1cb0cb3bd334bc2",
          "_projectId": "5847d23cd1cb0cb3bd334bf6",
          "_userId": "5109f1e918e6fcfc560001a6",
          "boundToObjectType": "post",
          "startDate": "2016-12-04T16:00:00.000Z",
          "updated": "2016-12-07T09:11:24.783Z",
          "created": "2016-12-07T09:11:24.783Z",
          "point": 1,
          "boundToObject": {
            "_id": "5847d23cd1cb0cb3bd334c3e",
            "_creatorId": "5109f1e918e6fcfc560001a6",
            "_projectId": "5847d23cd1cb0cb3bd334bf6",
            "postMode": "html",
            "source": "teambition",
            "tagIds": [],
            "visible": "members",
            "isArchived": null,
            "pin": false,
            "involveMembers": ["5109f1e918e6fcfc560001a6"],
            "updated": "2016-12-07T09:11:24.648Z",
            "created": "2016-12-07T09:11:24.648Z",
            "isDeleted": false,
            "attachments": [],
            "content": "content2",
            "title": "content2",
            "isShimoDoc": false,
            "url": "http://localhost/project/5847d23cd1cb0cb3bd334bf6/posts/post/5847d23cd1cb0cb3bd334c3e"
          }
        }]

