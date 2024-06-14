# few issues 

#### in patch add some example 

#### check the body parms in api
[check the body parms in api](https://photos.app.goo.gl/gy1UBGm1KRudPFK8A)
 
 ### incorrect schema 
```

/**
 * @swagger
 * paths:
 *   /tyre/admin/req/update/{id}:
 *     patch:
 *       tags:
 *         - ETS/tyre/admin/requestTyre
 *       summary: updateRequestTyre
 *       parameters:
 *         - name: id
 *           in: path
 *           required: True
 *           schema:
 *         - name: body
 *           in: body
 *           required: False
 *           schema:
 *             type: object
 *             properties:
                id:
                  type: number
                  required: True
                req_id:
                  type: integer
                  required: True
                req_date:
                  type: string
                  required: True
                base_location:
                  type: integer
                  required: True
                req_quantity:
                  type: integer
                  required: True
                req_by_user:
                  type: integer
                  required: True
                updated_by:
                  type: integer
                  required: True
 *       responses:
 *         '200':
 *           description: Success
 */

```
correct schema 



```

/**
 * 
 
 * @swagger
 * paths:
 *   /tyre/admin/req/update/{id}:
 *     patch:
 *       tags:
 *         - /tyre/admin/requestTyre
 *       summary: updateRequestTyre
 *       parameters:
 *         - name: id
 *           in: path
 *           required: true
 *           example: 1
 *           schema:
 *             type: integer
 *       requestBody:
 *         required: false
 *         content:
 *           application/json:
 *             schema:
 *               type: object
 *               properties:
 *                 req_id:
 *                   type: integer
 *                   required: true
 *                   example: 215623
 *                 req_date:
 *                   type: string
 *                   required: true
 *                   example: "2024-06-14"
 *                 base_location:
 *                   type: integer
 *                   required: true
 *                   example: 25
 *                 req_quantity:
 *                   type: integer
 *                   required: true
 *                   example: 20
 *                 req_by_user:
 *                   type: integer
 *                   required: true
 *                   example: 2
 *                 updated_by:
 *                   type: integer
 *                   required: true
 *                   example: 2
 *       responses:
 *         '200':
 *           description: Success
 */

```


### add eample in each api and in id it should be in Path Params 
#### i have share in above link or u can check in [here](https://photos.app.goo.gl/gy1UBGm1KRudPFK8A) 


#### use chatGpt prompt for spacing error and all 
