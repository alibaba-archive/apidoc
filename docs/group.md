## Group 群组

### 创建群组 [POST /api/groups]

新建群组，必须为组织成员

+ Attributes
    + _organizationId (ObjectID, required) - 组织 id
    + name (string, required) - 群组名称
    + userIds (array[ObjectID], required) - 群组成员 id，必须为组织成员，可为空

+ Request

        {
            "name": "X",
            "userIds": [
                "582ac0358a40417b939859e8"
            ],
            "_organizationId": "582ac0358a40417b939859e4"
        }

+ Response 200

        {
            "_id": "582acba5d530e4bc956b5054",
            "name": "X",
            "_organizationId": "582acba5d530e4bc956b5033",
            "_creatorId": "5109f1e918e6fcfc560001a6",
            "hasMembers": [
                {
                "_id": "582acba5d530e4bc956b5037",
                "avatarUrl": "",
                "name": "name2",
                "pinyin": "name2",
                "py": "name2",
                "isDefaultEmail": false
                },
                {
                "_id": "5109f1e918e6fcfc560001a6",
                "avatarUrl": "http://www.teambition.com/site_media/user_avatars/20120928112820_349.png",
                "name": "测试账号",
                "pinyin": "ce shi zhang hao",
                "py": "cszh",
                "isDefaultEmail": false
                }
            ],
            "created": "2016-11-15T08:47:33.567Z",
            "updated": "2016-11-15T08:47:33.567Z",
            "pinyin": "x",
            "py": "x"
        }

### 更新群组 [PUT /api/groups/{_groupId}]

必须为群组创建者或者组织管理员

+ Parameters
    + _groupId (ObjectId) - 群组 id

+ Attributes
    + name (string) - 群组名称

+ Request

        {
            "name": "Y"
        }

+ Response 200

        {
            "name": "Y",
            "updated": "2016-11-15T08:45:40.977Z",
            "_id": "582acb3487e24e9c95d72e80",
            "pinyin": "y",
            "py": "y"
        }

### 读取群组列表 [GET /api/organizations/{_organizationId}/groups]

+ Parameters
    + _organizationId (ObjectId) - 组织 id

+ Response 200

        [
            {
                "_id": "582ac5809ea2909094b38815",
                "name": "X",
                "_organizationId": "582ac57f9ea2909094b387f4",
                "_creatorId": "5109f1e918e6fcfc560001a6",
                "hasMembers": [
                {
                    "_id": "582ac5809ea2909094b387f8",
                    "avatarUrl": "",
                    "name": "name2",
                    "pinyin": "name2",
                    "py": "name2",
                    "isDefaultEmail": false
                },
                {
                    "_id": "5109f1e918e6fcfc560001a6",
                    "avatarUrl": "http://www.teambition.com/site_media/user_avatars/20120928112820_349.png",
                    "name": "测试账号",
                    "pinyin": "ce shi zhang hao",
                    "py": "cszh",
                    "isDefaultEmail": false
                }
                ],
                "created": "2016-11-15T08:21:20.527Z",
                "updated": "2016-11-15T08:21:20.527Z"
            }
        ]

### 删除群组 [DELETE /groups/{_groupId}]

必须为群组创建者或组织管理员

+ Parameters
    + _groupId (ObjectID) - 群组 id

+ Response 200

        {
            "_id": "582bd6b4adb18314b6fcff9e",
            "name": "Y",
            "_creatorId": "5109f1e918e6fcfc560001a6",
            "_organizationId": "582bd6b4adb18314b6fcff7b",
            "updated": "2016-11-16T03:47:01.149Z",
            "created": "2016-11-16T03:47:00.796Z",
            "py": "y",
            "pinyin": "y"
        }
