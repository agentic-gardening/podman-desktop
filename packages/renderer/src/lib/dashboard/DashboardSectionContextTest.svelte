<script lang="ts">
import { getContext } from 'svelte';

import { DASHBOARD_SECTION_CONTEXT, type DashboardSectionContext } from './dashboard-section-context';

const dashboard = getContext<DashboardSectionContext | undefined>(DASHBOARD_SECTION_CONTEXT);
</script>

<span aria-label="section context">{dashboard?.enhanced}</span>
