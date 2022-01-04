## Development notes
Some notes for planning / project details.

## Technologies

### Design
- Figma

### Front end
- NextJs
- React / typescript
- [Chakra UI](https://chakra-ui.com/)
- [Storybook](https://storybook.js.org/)
- Jest
- jest-axe (accessibility)
- Cypress

### Backend
- Express ([Integrated in NextJs](https://nextjs.org/docs/api-routes/introduction))
- [Jest](https://jestjs.io/)
- Swagger ([using next-swagger-doc](https://www.npmjs.com/package/next-swagger-doc))


## Storyboook driven development
> This workflow mimics the familiar practice of Test Driven Development (the first great Something-DD).
</br>[...]</br>
With Style-guide Driven Development, developers look at the UI as we code it. Instead of a test runner, developers are responsible for visually inspecting what we build and the style guide forms a set of visual expectations for what the UI should look like.

https://medium.com/nulogy/storybook-driven-development-a3c517276c07

## App details
The app should
- Let the user manage tasks that are linked to users.
- Let the user access to other users, their information and tasks.

Taks schema
```
{
    user_id: number,
    id: number,
    title: string,
    completed: boolean
}
```

User schema
```
{
    id: number,
    name: string,
    username: string,
    email: string,
        address: {
        street:  string,
        suite: string,
        city: string,
        zipcode: string,
        geo: {
            lat: number,
            lng: number
        }
    },
    phone: string,
    website: string,
    company: {
        name: string,
        catchPhrase: string,
        bs: string
    }
}
```

## Design
[Figma file](https://www.figma.com/file/VPbui8MdihVElzLgtPgZcY/experiment-app-tasks?node-id=0%3A1)