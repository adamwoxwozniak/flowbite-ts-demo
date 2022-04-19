<script>
  import "../app.css";
  import Sidebar from "flowbite-svelte";
  import {
    ChartPieIconSolid,
    ShoppingBagIconSolid,
    TableIconSolid,
    InboxInIconSolid,
    UserIconSolid,
    LoginIconSolid,
    CogIconSolid
  } from '@codewithshin/svelte-heroicons';

  let uid = 1;
  let links = [
    {
      id: uid++,
      name: 'Dashboard',
      href: '/',
      icon: ChartPieIconSolid
    },
    {
      id: uid++,
      name: 'E-commerce',
      icon: ShoppingBagIconSolid,
      href: '/',
      subtext: '3'
    },
    {
      id: uid++,
      name: 'Kanban',
      icon: TableIconSolid,
      href: '/',
      subtext: 'Pro'
    },
    {
      id: uid++,
      name: 'Inbox',
      icon: InboxInIconSolid,
      href: '/'
    },
    {
      id: uid++,
      name: 'Users',
      icon: UserIconSolid,
      href: '/'
    },
    {
      id: uid++,
      name: 'Sign In',
      icon: LoginIconSolid,
      href: '/'
    },
    {
      id: uid++,
      name: 'Setting',
      icon: CogIconSolid,
      href: '/'
    }
  ];
</script>

<Sidebar {links} />
<slot />
