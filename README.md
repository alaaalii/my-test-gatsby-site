Test repo for trying out the `gatsby-remark-grid-tables` plugin with Gatsby MDX

1. Run `yarn install` to install the required

1. Run `yarn develop` to start the server

1. Go to `localhost:8000/md-test` this is a page processed with `gatsby-transformer-remark` with the `gatsby-remark-grid-tables` plugin. You should see the Extended table render fine.

1. Go to `localhost:8000/mdx-test` this is a page processed with `gatsby-plugin-mdx` with the `gatsbyRemarkPlugins: ["gatsby-remark-grid-tables"]` option. You should see the Extended table is not rendered fine.

1. Stop the dev server, comment `gatsbyRemarkPlugins: ["gatsby-remark-grid-tables"]` and uncomment `remarkPlugins: [require("remark-grid-tables")]` then run the dev server again and visit `localhost:8000/mdx-test` - you will see the Extended table rendered fine.

I'm not sure why `gatsby-remark-grid-tables` doesn't work with `gatsbyRemarkPlugins`.
