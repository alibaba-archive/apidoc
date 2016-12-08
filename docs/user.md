## Group 用户

### 读取个人信息 [GET /api/users/me]

+ Response 200

        {
          _id: '56c437c31fd47955778026a7',
          email: 'test@tb.com',
          name: 'tester',
          avatarUrl: thumbnailUrl,
          created: '2016-02-17T09:05:07.514Z',
          title: '',
          birthday: null,
          location: '',
          phone: '',
          isActive: false,
          website: '',
          pinyin: 'tester',
          py: 't',
          isNew: false,
          notification:
          { comment: { mobile: true, email: false },
            newpost: { mobile: true, email: false },
            newtask: { mobile: true, email: false },
            newwork: { mobile: true, email: false },
            newevent: { mobile: true, email: false },
            involve: { mobile: true, email: false },
            update: { mobile: true, email: false },
            daily: { email: true },
            monthly: { email: true } },
          lastEntered: { web: null },
          aliens: [],
          strikerAuth: 'Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ1c2VySWQiOiI1NmM0MzdjMzFmZDQ3OTU1Nzc4MDI2YTciLCJleHAiOjE0NTU3ODYzMDcsInN0b3JhZ2UiOiJkZWZhdWx0In0.iXWin4SHf9lXrGSR4KDCABrDqkl4Jr23oe9iadHhkqo',
          phoneForLogin: '',
          enabledGoogleTwoFactor: false,
          emails:
          [ { email: 'test@tb.com',
              state: 1,
              _id: '56c437c31fd47955778026a8',
              id: '56c437c31fd47955778026a8' } ],
          snapperToken: 'eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ1c2VySWQiOiI1NmM0MzdjMzFmZDQ3OTU1Nzc4MDI2YTciLCJleHAiOjE0NTU4NzI3MDd9.cfFtsC2YxlmQ6udUP8mwiq6dQisqddUMfLquCIORTiQ',
          locationByIP: { country: '', region: '', city: '' },
          badge: 0,
          inbox: 0,
          normal: 0,
          ated: 0,
          later: 0,
          private: 0,
          hasNormal: false,
          hasAted: false,
          hasLater: false,
          hasPrivate: false,
          calLink: 'webcal://localhost:5000/api/events/ecb07e3983e94a3d7dc5aa80751d4086f2bb0165cb28d8bf1116f37794ecf6e5.ics',
          taskCalLink: 'webcal://localhost:5000/api/tasks/53353243a8c1f74bf3fae41e2cad0404e290d65d5620e8fe0dd52d05fde7409e.ics',
          joinedProjectsCount: 0
        }

